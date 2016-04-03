---
layout: reference
title: "Reference"
---

<!--original
---
layout: reference
title: "Reference"
---
-->

# ���t�@�����X

<!--original
# Reference
-->

Kotlin�����[�W�����C�u����](/api/latest/jvm/stdlib/index.html)�̊��S�ȃ��t�@�����X��񋟂��܂��B

<!--original
Provides a complete reference to the Kotlin language and the [standard library](/api/latest/jvm/stdlib/index.html).
-->

### �ǂ�����n�߂�Ηǂ���

<!--original
### Where to Begin
-->

���̃��t�@�����X�́A���Ȃ����ȒP�ɐ����Ԃ�Kotlin���w�ׂ�悤�݌v����Ă��܂��B��{�I�ȍ\������n�߁A��荂�x�ȃg�s�b�N�ɐi�݂܂��B�ǂ�ł���ԁA[�I�����C��IDE](http://try.kotlinlang.org/)�ŗ���������Ƃ��ł��܂��B

<!--original
This reference is designed for you to easily learn Kotlin in a matter of hours.
Start with the [basic syntax](basic-syntax.html), then proceed to more advanced topics.
While reading, you can try out the examples in the [online IDE](http://try.kotlinlang.org/).
-->

Kotlin���ǂ̂悤�Ȃ��̂��킩������A[Kotlin Koans](/docs/tutorials/koans.html) �i�C���^���N�e�B�u�ȃv���O���~���O���K�j�ɒ��킵�Ă݂Ă��������BKoan�̉�@���킩��Ȃ��A�܂��͂��G���K���g�ȉ�@�����T���̏ꍇ�́AKotlin��[�C�f�B�I��](idioms.html)���`�F�b�N���Ă��������B

<!--original
Once you get an idea of what Kotlin looks like, try yourself in solving some [Kotlin Koans](/docs/tutorials/koans.html) - interactive programming exercises.
If you are not sure how to solve a Koan, or you're looking for a more elegant solution, check out [Kotlin idioms](idioms.html).
-->


### �I�t���C���u���E�Y
���t�@�����X�S�̂̃h�L�������g��1��[PDF�t�@�C��]({{ site.pdf_url }})�Ƃ��ă_�E�����[�h���邱�Ƃ��ł��܂��B

<!--original
### Browse offline
You can download the entire reference documentation as a single [PDF file]({{ site.pdf_url }}).
-->

# ����

<!--original
# Books
-->

## Kotlin in Action

<!--original
## Kotlin in Action
-->

   <a href="https://manning.com/books/kotlin-in-action"><img src="{{ site.baseurl }}/assets/images/Jemerov-Kotlin-MEAP-HI.png" style="float: left; margin-right: 10px; margin-bottom: 10px;"></a>

<!--original
   <a href="https://manning.com/books/kotlin-in-action"><img src="{{ site.baseurl }}/assets/images/Jemerov-Kotlin-MEAP-HI.png" style="float: left; margin-right: 10px; margin-bottom: 10px;"></a>
-->

[Kotlin in Action](https://manning.com/books/kotlin-in-action)��Kotlin�`�[���̊J���҂ł���Dmitry Jemerov��Svetlana Isakova�Ɏ��M����܂����B 
���̖{��MEAP�v���O�����Ŏ�ɓ���܂��B���̃v���O�����ł͖{���͖��ɏ����������A�͒P�ʂœǂ߂�悤�ɂȂ��Ă����A�Ō�ɖ{�S�̂��������܂��B

<!--original
[Kotlin in Action](https://manning.com/books/kotlin-in-action) is a book on Kotlin being written by Dmitry Jemerov and Svetlana Isakova,
developers on the Kotlin team. The book is currently available through the MEAP program, which allows you to read the book
chapter-by-chapter while it is being written and get the final book when it is finished.
-->

�N�[�|���R�[�h�u39jemerov�v���g�p����ƁA39�������œ���ł��܂��B

<!--original
Use the coupon code '39jemerov' to get a 39% discount code on the book.
-->

<h2 style="clear: left">Kotlin for Android Developers</h2>

<!--original
<h2 style="clear: left">Kotlin for Android Developers</h2>
-->

  <a href="https://leanpub.com/kotlin-for-android-developers"><img src="{{ site.baseurl }}/assets/images/kotlin-for-android-developers.png" style="float: left; margin-right: 10px; margin-bottom: 10px;"></a>

<!--original
  <a href="https://leanpub.com/kotlin-for-android-developers"><img src="{{ site.baseurl }}/assets/images/kotlin-for-android-developers.png" style="float: left; margin-right: 10px; margin-bottom: 10px;"></a>
-->

Antonio Leiva��������[Kotlin for Android Developers](https://leanpub.com/kotlin-for-android-developers)�ł́AKotlin���g����Android�A�v�����X�N���b�`����쐬�����@���Љ�Ă��܂��B

<!--original
[Kotlin for Android Developers](https://leanpub.com/kotlin-for-android-developers) is a book by Antonio Leiva showing
how Kotlin can be used for creating an Android application from scratch.
-->

<script src="http://code.jquery.com/jquery-1.11.0.min.js"></script>
<script>
$(function() {
  $("*").contents().filter(function() {
    return this.nodeType==8 && this.nodeValue.match(/^original/);
  }).each(function(i, e) {
    var tooltips = e.nodeValue.replace(/^original *[\n\r]|[\n\r]$/g, '');
    $(this).prev().attr('title', tooltips);
  });
});
</script>
