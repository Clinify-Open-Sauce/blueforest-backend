# blueforest-backend

## Crete New User
id is created automatically 

```
mutation createMutation {
  createUser(userData: {discordId: {put discord id here}, discordTag: {put discord tag like this "TIlak#7891"}, avatar: {put link of the image here} , status: {true,False}, xp: {put int here}, coins: {put integer here}, tressUnlocked: [1,2,3]}) {
    user {
      discordId
      discordTag
      avatar
      status
      xp 
      coins
      tressUnlocked{
        treeId
        treeName
      }
    }
  } 
}
```

## to get all users 
```
query
{
  allUsers
  {
    discordId
    discordTag
    tressUnlocked
    {
      treeId
      treeUrl
      treeName

    }
  }
}
```
## to get user by id 
```



