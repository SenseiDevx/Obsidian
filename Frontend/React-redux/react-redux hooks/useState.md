`useState` - это хук (hook) в React, который позволяет создавать состояние (state) в функциональном компоненте.

Хук `useState` принимает начальное значение состояния и возвращает массив из двух элементов: текущее значение состояния и функцию, которая позволяет изменять это значение.

Например, рассмотрим компонент, который выводит количество кликов по кнопке:
import { useState } from 'react';

function Button() {
  const [count, setCount] = useState(0);

  function handleClick() {
    setCount(count + 1);
  }

  return (
    <div>
      <button onClick={handleClick}>Click me</button>
      <p>You clicked the button {count} times</p>
    </div>
  );
}
В этом компоненте мы используем хук `useState` для создания состояния `count`, который изначально равен 0. Затем мы используем функцию `setCount` для изменения значения `count` при клике на кнопку.

Функция `setCount` принимает новое значение `count`, которое заменит предыдущее значение. React затем обновляет интерфейс, отображая новое значение `count` в параграфе.

Важно понимать, что при использовании `useState` значение состояния не изменяется напрямую, а только через вызов соответствующей функции. Также, при каждом изменении состояния, React автоматически перерисовывает компонент, чтобы отобразить новое значение состояния.

[[react hooks]]