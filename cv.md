# Elena Vileishikova
**Curriculum Vitae** / **last update: 08.11.2023**
### Summary:

### Contacts:
  - **e-mail:** [vilejshikova@gmail.com](mailto:vilejshikova@gmail.com)
  - **discord:** [Aliona#7409](https://discordapp.com/users/1122842754175742052/)
  - **github:** [@Alv0425](https://github.com/Alv0425)
  - **telegram:** [@Alv0425](https://t.me/Alv0425)
  
### Education:
 - **2010-2015: Belarusian State University, Faculty of Physics (dep. of Laser Physics & Spectroscopy)**
 - **2015-2019: Belarusian National Technical University (master and postgraduate)**
   #### Courses (JS):
 - **[FreeCodeCamp](https://www.freecodecamp.org/)** (in progress)
 - **RS Schools: Course «JavaScript/Front-end. Stage 0»** ([certificate](https://app.rs.school/certificate/j77h435w))
 - **RS Schools: Course «JavaScript/Front-end. Stage 1»** (in progress)

### Skills:
  - **Programming skills[^1]:** MATLAB, Python, C, JS 
  - **Markup**: HTML, Markdown
  - **SSLs & preprocessors**: CSS, SCSS[^1]
  - **VCS**: git, github

### Code example:
[Codewars kata: Matrix Determinant](https://www.codewars.com/kata/52a382ee44408cea2500074c): Write a function that accepts a square matrix (N x N 2D array) and returns the determinant of the matrix.

```javascript
  function determinant(m) {
    const getMinor = (matrix, index) => {
      let size = matrix.length;
      return matrix.slice(1, size).map((el) => {
        return el.slice(0, index).concat(el.slice(index + 1, size));
      });
    }
    const size = m.length;
    if (size === 1) {
      return m[0][0];
    } 
    if (size === 2) {
      return (m[0][0] * m[1][1]) - (m[0][1] * m[1][0]);
    }
    if (size >=3) {
      let det = 0;
      for (let i = 0; i < size; i++) {
        det += ((-1) ** i) * m[0][i] * determinant(getMinor(m, i));
      }
      return det;
    }
  }

```
### Languages: 
- **English** - Intermediate[^2] 
- **Belarusian** - Native
- **Russian** - Native
- **Polish** - Basic

[^1]: Limited experience
[^2]: I have some practical experience via communication with colleagues, participatig in conferences, writing articles etc.