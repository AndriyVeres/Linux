## FILESYSTEM PARTITIONS, ACCORDING TO FHS RECOMMENDATIONS

### /tmp
>*must be on another partition, than root catalogue, in case of very often read activities*

### /use
>*must be on another partition, because it doesn`t require write operations*

### /var
### /home
>*must be on anothers partition in case of non-determined size, overflow based bugs, in case if we will not place them on another partition brings some surprised, when all root catalogue partition will be overloaded*