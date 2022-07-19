# LoopForMerging2F-2R

#for loop for merging 2F or 2R files and save in another directory



    for i in {1..N};

    do

    cat *_NAME${i}_*_1.fastq.gz > /DESTINATION PATH/NAME{i}_R1.fastq.gz

    cat *_NAME${i}_*_2.fastq.gz > /DESTINATION PATH/NAME{i}_R2.fastq.gz

    done


#Example using bacterial WGS data: 

#file name format is as: *_EC1_*_1.fastq.gz for forward read and it is similar for reverse. The file's number is from 1 to 2019 as the last forward file is EC2019

    for i in {1..2019};

    do

    cat *_EC${i}_*_1.fastq.gz > /media/mahnaz/merged/EC${i}_R1.fastq.gz

    cat *_EC${i}_*_2.fastq.gz > /media/mahnaz/merged/EC${i}_R2.fastq.gz

    done
