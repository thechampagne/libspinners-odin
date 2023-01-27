# libspinners-odin

[![](https://img.shields.io/github/v/tag/thechampagne/libspinners-odin?label=version)](https://github.com/thechampagne/libspinners-odin/releases/latest) [![](https://img.shields.io/github/license/thechampagne/libspinners-odin)](https://github.com/thechampagne/libspinners-odin/blob/main/LICENSE)

Odin binding for **libspinners** an elegant terminal spinners.

### Example

```odin
import "core:time"
import "spinner"

main :: proc() {
    spin := spinner.new(spinner.spinner_spinners_t.Dots9, "Waiting for 3 seconds")
    time.sleep(3e+9)
    spinner.stop(&spin)
    spinner.clean(&spin)
}
```

### References
 - [libspinners](https://github.com/thechampagne/libspinners)

### License

This repo is released under the [MIT](https://github.com/thechampagne/libspinners-odin/blob/main/LICENSE).
