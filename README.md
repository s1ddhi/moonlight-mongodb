# Moonlight MongoDB

Docker MongoDB container for [moonlight](https://github.com/s1ddhi/moonlight).

This stores data in the DB in a local volume in `./mongodb/ledger` so restarts will maintain data previously added.

## Deployment

```
sudo docker exec -it mongodb bash
```

To execute the docker container.

## Interactions

```
mongosh
```

To launch the MongoDB CLI.

## Collections

- `apys`

This stores fetched daily APYs from Convex's off-chain oracle.

- `ledger`

This stores all deposit and withdrawal requests submited by the backend [moonlight](https://github.com/s1ddhi/moonlight).

- `userBalances`

This tracks user balances in terms of base balance (LP balance) and interest accrued.