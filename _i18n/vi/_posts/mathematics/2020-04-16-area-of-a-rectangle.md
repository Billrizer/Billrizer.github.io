---
layout: post
categories: mathematics
title: Làm sao để tính được diện tích của một hình chữ nhật?
description: Xoay quanh việc tính diện tích của một hình quen thuộc
language: vi
---


Đọc bài này thì coi như các vị huynh đài đây đã biết ```hình chữ nhật``` là gì rồi nhé.  
Bài viết này mình sẽ viết về diện tích của ```hình chữ nhật```, tại sao diện tích của hình chữ nhật lại là tích của hai cạnh với nhau.  
Công thức tính diện tích của ```hình chữ nhật``` đã được đề cập trong các sách giáo khoa bậc Tiểu học, tuy nhiên mình cũng chưa bao giờ thắc mắc tại sao diện tích của hình đó lại là tích của hai độ dài. Mãi cho đến khi học sinh của mình hỏi thì mình mới nghĩ đến điều này.

- Table of content
{:toc}

## Diện tích là gì

Đầu tiên mình sẽ cần có định nghĩa của diện tích trước.

> Diện tích là độ đo dùng để đo độ lớn của bề mặt, là số đo phần mặt phẳng bị giới hạn bởi một hình

Nói một cách dễ hiểu, diện tích là phần bề mặt bị vật chiếm chỗ.

Việc có những quy ước cơ bản là điều cần thiết, ví dụ như thế nào là `1m, 1l,1kg,...` thì ở đây mình cũng có quy ước của 1 đơn vị diện tích.  

> 1 đơn vị diện tích là diện tích của hình vuông cạnh 1 đơn vị độ dài

## Phần chính

### 1. Hình chữ nhật có cạnh là số nguyên ($$\mathbb{Z}$$)

Đôi với những hình chữ nhật có các cạnh là số nguyên, câu chuyện rất đơn giản. Ta chỉ việc lấp đầy ```hình chữ nhật``` đó bằng các hình vuông đơn vị, lúc đó, diện tích của ```hình chữ nhật``` sẽ đúng bằng số hình vuông đơn vị được sử dụng.

<img src="/post_image/mathematics/2020-04-16-area-of-a-rectangle.assets/rect_integer.png" alt="rect_integer" style="zoom:24%;" />

### 2. Hình chữ nhật có cạnh là số hữu tỉ ($$\mathbb{Q}$$)

Những ```hình chữ nhật``` có độ dài cạnh là các số hữu tỉ cũng đơn giản thôi. Giả sử rằng cần tính diện tích của ```hình chữ nhật``` có các cạnh là $$\displaystyle \frac{a}{c}, \frac{b}{d}$$.  Ta sẽ xếp $$cd$$ hình này lại để thu được một hình chữ nhật có kích thước $$a\times b$$. 

<img src="/post_image/mathematics/2020-04-16-area-of-a-rectangle.assets/rect_quotient.png" alt="rect_quotient" style="zoom:24%;" />

Theo như phần trên, diện tích của hình chữ nhật này là $$S' = ab$$, mà hình này lại được ghép bởi $$cd$$ hình chữ nhật bằng nhau, vậy nên diện tích của mỗi hình chữ nhật kích thước $$\frac{a}{c} \times \frac{b}{d}$$ là


$$
\begin{aligned}
S = \frac{ab}{cd} = \frac{a}{c} \times \frac{b}{d}
\end{aligned}
$$

Dễ đúng không?

### 3. Hình chữ nhật có cạnh là số thực ($$\mathbb{R}$$)

```Hình chữ nhật``` có các kích thước là số thực thì phức tạp hơn một chút. Hiển nhiên ta không thể dùng cách chia, ghép hình như đã làm với số hữu tỉ, ví dụ với hình chữ nhật có kích thước $$\sqrt{2} \times \sqrt{3}$$ chẳng hạn. Khi đó. việc chia ghép hình trở nên khó thực hiện hơn, và mình nghĩ là cần phải tìm một hướng thực hiện khác.

Khá là may mắn khi mà mình nhớ ra được một điều khá hay ho từ hồi mình còn học THPT:

> Mỗi một số thực đều tồn tại một dãy hữu tỉ hội tụ đến nó

Thực chất, tính chất trên chính là tính ```trù mật``` của $$\mathbb{Q}$$ trong $$\mathbb{R}$$, tức là, với mỗi một số thực $$x \in \mathbb{R}$$, luôn luôn tồn tại một dãy số $$\{x_n\} \subset \mathbb{Q}$$ sao cho $$\underset{n \to \infty}{\lim}x_n = x$$.

> Nếu các tráng sĩ có quan tâm đến chứng minh của mệnh đề trên, thì mình sẽ viết ở bài sau

Mục đích của ta sẽ là tìm ra một dãy các hình chữ nhật có các cạnh hữu tỉ và kích thước gần với kích thước của hình chữ nhật cần tính. 

Giả sử ta cần tính diện tích của một hình có kích thước $$x \times y$$, trong đó $$x, y \in \mathbb{R}$$. Khi đó, sử dụng bổ đề, hiển nhiên tồn tại các dãy số hữu tỉ hội tụ về $$x, y$$. Giả sử $$\{x_n\}, \{u_n\}$$ là 2 dãy đơn điệu tăng, giảm theo thứ tự và có $$\underset{n \to \infty}{\lim}x_n = \underset{n \to \infty}{\lim}u_n = x$$; $$\{y_n\}, \{v_n\}$$ là 2 dãy đơn điệu tăng, giảm theo thứ tự và có $$\underset{n \to \infty}{\lim}y_n = \underset{n \to \infty}{\lim}v_n = y$$.

<img src="/post_image/mathematics/2020-04-16-area-of-a-rectangle.assets/rect_real.png" alt="rect_real" style="zoom:24%;" />

Theo đó, dễ dàng nhận thấy rằng $$x_{i}y_{i} \le xy \le u_{i} v_{i}, \forall i \in \mathbb{N}$$, tức là nếu gọi diện tích của hình chữ nhật kích thước $$x_i, y_i$$ và $$u_i, v_i$$ lần lượt là $$S_i$$ và $$X_i$$; diện tích của hình cần tính là $$S$$, thì khi đó ta luôn có:

$$
\begin{aligned}
S_i \le S \le X_i, \forall i \in \mathbb{N}
\end{aligned}
$$


Lấy giới hạn vào các vế của bất đẳng thức, ta có:

$$
\begin{aligned}
& \underset{i \to \infty}{\lim}S_i \le S \le \underset{i \to \infty}{\lim}X_i \\
\Leftrightarrow & \underset{i \to \infty}{\lim}x_i y_i \le S \le \underset{i \to \infty}{\lim}u_i v_i
\end{aligned}
$$

Mặt khác, ta có

$$
\begin{cases}
\underset{i \to \infty}{\lim}{x_i y_i} = \underset{i \to \infty}{\lim}{x_i} \underset{i \to \infty}{\lim}{y_i} = xy \\
\underset{i \to \infty}{\lim}{u_i v_i} = \underset{i \to \infty}{\lim}{u_i} \underset{i \to \infty}{\lim}{v_i} = xy
\end{cases}
$$


Điều này có nghĩa là $$xy \le S \le xy$$, chứng tỏ $$S = xy$$.

Yo, điều này có nghĩa là ta đã chứng minh được diện tích của một hình chữ nhật có cạnh $$x, y \in \mathbb{R}$$ thì sẽ có diện tích $$S = xy$$.

## Tổng kết

Chốt lại, là một vấn đề tưởng chừng hiển nhiên nhưng lại không được hiển nhiên cho lăm. Kết thúc một ngày suy nghĩ, tối chuẩn bị đi dạy để trả lời học sinh.

Mình đi học đến nay là 15 năm, chưa một lần nào mình thắc mắc những câu như này.

Có những điều tưởng như hiển nhiên mà đôi khi lại không hiển nhiên lắm

Chào thân ái và quyết thắng!