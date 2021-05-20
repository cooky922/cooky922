- 👋 Hi, I’m @cooky922
- 👀 I’m interested in C++
- 🌱 I’m currently learning C++
- 💞️ I’m looking to collaborate on myself
- 📫 How to reach me ...

<!---
cooky922/cooky922 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
## What I Like in C++
* Seems very easy to me.
* Data Structure and Algorithm are not my taste (currently).
* I loved templates!
* There are many things you could possibly do!

## What I Hate in C++
* Frustrating at making big projects 
* I've been waiting for `std::format` and full support of modules.

## I've been forking some of the repositories :>

## My Favorite Source Code
#### Fibonacci 
```c++
template <std::integral T>
constexpr T fib(T n) {
    auto phi = std::numbers::phi_v<long double>;
    return std::round((std::pow(phi, n) - std::pow(-phi, -n)) / std::sqrt(5.0L));
}
```
#### Eh... I don't know! :>
```c++
[] -> decltype(auto) { return std::cout << "Hello "; }() << "world!";
```

#### Custom Property Class (unfinished)
```c++
template <typename T>
class property {
private:
    T value;
public:
    property(T& value_) : value{value_} {}

    // set
    property<T>& operator=(const T& value_) {
        value = value_;
        return *this;
    }

    // get
    operator const T&() const {
        return value;
    }

    // lexicographical compare
    const bool operator<=>(const property<T>&) const = default;

    // input / output
    friend std::ostream& operator<<(std::ostream& os, const property<T>& prop) {
        os << prop.value;
        return os;
    }
    friend std::istream& operator>>(std::istream& is, const property<T>& prop) {
        is >> prop.value;
        return is;
    }

};
```

