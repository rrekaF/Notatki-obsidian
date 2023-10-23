#Code #Unity #GameDev 
## Changing position
Adjust the settings in **Edit > Project settings > Input manager**
```cs
float horizontal = Input.GetAxis("Horizontal");
float vertical = Input.GetAxis("Vertiacl");
// Gets the position from the game
Vector2 position = transform.position;
// Changes the position (right -> horizontal = 1, left -> horizontal = -1)
position.x = position.x + 0.1f * horizontal * Time.deltaTime; //   * Time.deltaTime makes the 
position.y = position.y + 0.1f * vertical * Time.deltaTime; //     movement frame independent
// Applies the changes to the game
transform.position = position;
```
