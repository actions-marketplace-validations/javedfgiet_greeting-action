# greeting-action
#Simple custom action for demo learning
**Simple Greeting Action** is a lightweight custom Githib Action designed to demonstrate how composite action works.
This action accept a user's name and environment as inputs, prints a greeting message, and exposes a reusable output that can be consumed in subsequent workflow steps

It is intentionally simple, making it ideal for:
- Learning custom action structure
- Teaching composite action concept in CI/CD
- Dmonstrating inputes, outputs and step execution
## What this action does
 - Takes a **username** as imput **mandatory**
 - Takes a **season** as input as `Summer, Winter, Rainy - **optional**, default season is **summer**
 - Print a greeting message
 - Return output value calles `message`.

## Sample usage
```
 - name: Greeting
   id: greet
   uses: ./
   with:
     username: javedfgiet
     season: winter
```
