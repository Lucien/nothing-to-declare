# Nothing to Declare
Swift Library for validation and generation of CPF and CNPJ numbers.

# Features

- CPF validation
- CPF generation
- CNPJ validation
- CNPJ generation
- Accepts plain or masked number as input.
- CPF has information about the fiscal region and brazilian states associated.
- CNPJ shows if the number is from a company headquarters (0001 before the verification digits).

# Usage


## Validation

```swift
    do {
        let cpf = try CPF(number: "51135733961")
        cpf.isValid() // true
    } catch Parser.InputError.invalidFormat {
        print("invalid CPF format")
    }
```

## Generation

```
let cpf = CPF.generate()
```

Check out more on [Playgrounds](README.playground)

# Memes
![](https://static.poder360.com.br/2024/03/prismada-irpf-memes-1-15mar2024.png)
![](https://static.poder360.com.br/2024/03/prismada-irpf-memes-3-15mar2024.png)
![](https://i.pinimg.com/736x/ce/fd/57/cefd57f6b5e2ac84db7496e3f4c031e2.jpg)
