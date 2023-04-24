# Lab Report 2

![Image](lr21.jpg)

## Part 1

![Image](lr22.jpg)
![Image](lr23.jpg)

In my code, when I run this the methods used are:

### handleRequest

handleRequest takes an argument of type URI. The value of String s and int cnt are relevant and change. Depending on how handleRequest handles the request, s's value could add another String value and cnt's value could increase by 1.

### getPath

getPath does not take any arguments. When getPath is called, the URI parameter is the only field that is relevant because the method reads the path based on the value of that field. The value does not change though because this method simply reads a specific segment of the String.

### getQuery

getQuery is similar to getPath and does not require any arguments but relies on the URI type parameter. This field is relevant because the method reads the query based on the value of that field. The value does not change though because this method simply reads a specific segment of the String. Although, if the query were to include an actual query value, then that value would be added to the String s value.

## Part 2

### Failure-inducing input:

```

  @Test
  public void testReversed() {
    int[] input1 = {1,2,3};
    assertArrayEquals(new int[]{0}, ArrayExamples.reversed(input1));
  }

```

### Input that doesn't induce failure:

```
  @Test
  public void testReversed() {
    int[] input1 = {0};
    assertArrayEquals(new int[]{0}, ArrayExamples.reversed(input1));
  }
```
### Output with failure-inducing

![Image](lr24.jpg)

### Output with input that does not induce failure

![Image](lr25.jpg)

### Before code:

```
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
```

### After code:
```
 static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
```

## Part 3

I didn't know I could code a website using Java like that. I've made html websites with css and JavaScript but using Java with its object-oriented stuff is cool. 


