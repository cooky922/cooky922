- 👋 Hi, I’m @cooky922
- 👀 I’m interested in C++
- 🌱 I’m currently learning C++
- 💞️ I’m looking to collaborate on myself
- 📫 How to reach me ...

<!---
cooky922/cooky922 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

## My Favorite Source Code
```c++
template <std::integral T>
constexpr T fib(T n) {
    auto phi = std::numbers::phi_v<long double>;
    return std::round((std::pow(phi, n) - std::pow(-phi, -n)) / std::sqrt(5.0L));
}
```
