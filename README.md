# Unidecode

ASCII transliterations of Unicode text. Julia port of [https://github.com/avian2/unidecode](https://github.com/avian2/unidecode). Name changed to avoid conflict with [Unidecode.jl](https://github.com/matthieugomez/Unidecode.jl).


## Installation

    pkg> add https://github.com/wswu/unidecode


## Usage

    julia> translit("你好")
    "Ni Hao "

    julia> translit('30 \U0001d5c4\U0001d5c6/\U0001d5c1')
    "30 km/h"
    
Function signature:

    unidecode(str, errors="ignore", replace_str="?")