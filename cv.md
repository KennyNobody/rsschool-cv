# Egor Badulin
### Contacts
Telegram: [Kenny_Nobody](https://t.me/Kenny_Nobody)

Email: [nobodykenny@gmail.com](mailto:nobodykenny@gmail.com)

### Code example
```
document.addEventListener('DOMContentLoaded', () => {
    let menu = document.querySelector('[data-menu]');
    menu ? webApp.menu = new Menu(menu) : false;
});

class Menu {
    constructor(el) {
        this.el = el;
        this.opened = false;
        this.buttons = document.querySelectorAll('[data-menu-button]');
        this.setListeners();
    }
    setListeners = () => {
        for (let item of this.buttons) {
            item.addEventListener('click', () => {
                this.openMenu();
            })
        }
    }
    openMenu = () => {
        if (this.opened == false) {
            this.el.classList.add('menu--visible');
            this.opened = true;
        } else {
            this.el.classList.remove('menu--visible');
            this.opened = false;
        }
    }
}
```

### Languages
- Russian (native)
- English (pre-intermediate)