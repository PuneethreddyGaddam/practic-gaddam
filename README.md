# practic-gaddam

# Puneeth Reddy

###### I do not have a favorite band, but I really like Hans Zimmer

-----
I like him because his music sounds very **strong** and emotional, especially in movies. His music makes scenes feel more serious and exciting, even without people talking. I also like how his music creates **suspense** and keeps me interested. Sometimes I listen to his music while studying because it helps me focus.

-------

### Favorite Musicians
1. Hans Zimmer
2. Thaman 
3. Krem

### Favorite Books
- Atomic Habits
- The Alchemist
- Rich Dad Poor Dad

----

[Read about my favorite place to visit: Bali](MyLocation.md)


-----

## Places I Would Like to Visit

Below is a table of places I would like to visit in the future. These locations
interest me because of their culture, history, and unique experiences they offer.

| Place        | Reason for Visit                     | Distance from Home | Weekly Budget ($) |
|--------------|--------------------------------------|-------------------|-------------------|
| Bali         | Beaches and cultural experiences     | 9,000 miles       | 2800              |
| Paris        | Art, culture, and history            | 3,600 miles       | 2500              |
| Tokyo        | Technology and traditional culture   | 6,700 miles       | 3000              |
| Rome         | Ancient architecture and landmarks   | 4,800 miles       | 2300              |


## Favorite Quotes

>  "Love is the one thing that transcends time and space." 

*Hans Zimmer*

> "We used to look up at the sky and wonder at our place in the stars."

*Hans Zimmer*

-----

### Code Fencing

This code snippet demonstrates an immutable `User` class written in Dart. The class uses `final` variables, which means the values cannot be changed once the object is created. To update values, the `copyWith` method creates a new `User` object with modified data. The equality operator and `hashCode` are overridden so that objects are compared based on their values.


```dart
@immutable
class User {
    final String name;
    final int age;

    User(this.name, this.age);

    User copyWith({
        String? name,
        int? age,
  }) {
    return User(
    name ?? this.name,
    age ?? this.age,
    );
  }
  @override
  bool operator ==(Object o) {
    if (identical(this, o)) return true;

    return o is User && o.name == name && o.age == age;
  }

  @override
  int get hashCode => name.hashCode ^ age.hashCode;
}


### Link of snippet source : https://dart.pieces.cloud/?p=1a63488211
