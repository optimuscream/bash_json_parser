#!/bin/bash

while read -r col ; do
        echo -e "\t{"
        echo -e "\t\t"\"name\"": "\"$col\"","
        echo -e "\t\t"\"value\"": "\"$col\"""
        echo -e "\t},"
done | sed -e '1i [' -e '$a ]' | tac | sed '2s/},/}/' | tac
