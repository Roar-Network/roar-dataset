# Roar-dataset

It was necesary to create an artificial dataset to train:

- classifier of roars
- recommenders of roars
- sentiment analizer of roars

Roar dataset is based on Yahoo Answers Topic. Each roar belong to one of the following categories:

1. Society & Culture
2. Science & Math
3. Health
4. Education
5. Computer & Internet
6. Sports
7. Business & Finance
8. Entretainment
9. Family
9. Governemnt & Politic

## How was created Roar dataset?

> A roar is a short text of at least 512 characters.

Then, as first step, we take as a roar each title + answer of Yahoo Answer Topic. Only which has at least 512 characters.

In addition, create a preference probabilistic graph, which represent what is the probability of user i which like category k, like category n, where n != k.

Then, we create 5000 users. A user is generated adding k random preference array with differents main categories.

Then, select most liked categories for a user, and select randomly roars and rate them. 