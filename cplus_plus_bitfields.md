What is the use of a bit field in C++ ?

> Bit fields can be used to reduce memory consumption when a program requires 
> a number of integer variables which always will have low values. For example, 
> in many systems storing an integer value requires two bytes (16-bits) of memory; 
> sometimes the values to be stored actually need only one or two bits.

[wikipedia](https://en.wikipedia.org/wiki/Bit_field)

> Declares a class data member with explicit size, in bits. Adjacent bit field 
> members may be packed to share and straddle the individual bytes. 

[cppreference](https://en.cppreference.com/w/cpp/language/bit_field)

    struct halfbyte_t {
        unsigned int half1: 4;
        unsigned int half2: 4;
    } halfbyte;

[stackoverflow](https://stackoverflow.com/questions/35857111/c-how-to-use-bitfields)


