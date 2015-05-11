# Python
from pyparsing import oneOf, Literal, Word, alphas, nums, ZeroOrMore
greeting = oneOf("Hello Ahoy Yo Hi") + Literal(",") + Word(alphas) + ZeroOrMore(Word(nums))+ Literal("!")
print(greeting.parseString("Hello, World!"))
