# [WIP] DOCTOSHOTGUN

This script lets you automatically book a vaccine slot on Doctolib for Berlin.


<p align="center">
  <img src="https://raw.githubusercontent.com/rbignon/doctoshotgun/da5f65a1e2ecc7b543376b1549c62004a454b90d/example.svg">
</p>

## How to use it

Install dependencies:

```
pip install -r requirements.txt
```

Run:

```
./doctoshotgun.py <email> [password]
```

Optional arguments:

```
--patient <index>                                       : select patient for which book a slot
--debug                                                 : display debug information
```

### Select patient

For doctolib accounts with more thant one patient, you can select patient just after launching the script:

```
$ ./doctoshotgun.py paris roger.philibert@gmail.com PASSWORD
Available patients are:
* [0] Roger Philibert
* [1] Luce Philibert
For which patient do you want to book a slot?
```

You can also give the patient id as argument:

```
$ ./doctoshotgun.py roger.philibert@gmail.com PASSWORD -p 1
Starting to look for vaccine slots for Luce Philibert...
```

## Credit

[Original Owner](https://github.com/rbignon/doctoshotgun)
