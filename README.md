# BottomSheet
Tutorial Membuat BottomSheet Dialog unsur fragment

### Features

- Menampilkan panel berbentuk frame layout
- Memberikan Effect Alpha atau transparansi layer hitam
- Behavior slide ke atas dan bawah

# Sample

![](https://raw.githubusercontent.com/michaelbel/BottomSheet/master/screenshots/bs_light_3.png)

![](https://img.shields.io/github/stars/pandao/editor.md.svg) ![](https://img.shields.io/github/forks/pandao/editor.md.svg) ![](https://img.shields.io/github/tag/pandao/editor.md.svg) ![](https://img.shields.io/github/release/pandao/editor.md.svg) ![](https://img.shields.io/github/issues/pandao/editor.md.svg) ![](https://img.shields.io/bower/v/editor.md.svg)


**Library**

	implementation 'com.google.android.material:material:1.1.0'

#### Kode XML (bottom_sheet.xml)

```xml
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:paddingBottom="8dp" >
    <TextView
        android:id="@+id/textView"
        android:layout_marginTop="8dp"
        android:drawableLeft="@drawable/ic_share"
        android:drawableStart="@drawable/ic_share"
        android:text="@string/action_share"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        style="@style/ActionItem"
        />
    <TextView
        android:id="@+id/textView2"
        android:drawableLeft="@drawable/ic_upload"
        android:drawableStart="@drawable/ic_upload"
        android:text="@string/action_upload"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView"
        style="@style/ActionItem"
        />
    <TextView
        android:id="@+id/textView3"
        android:drawableLeft="@drawable/ic_copy"
        android:drawableStart="@drawable/ic_copy"
        android:text="@string/action_copy"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView2"
        style="@style/ActionItem"
        />
    <TextView
        android:id="@+id/textView4"
        android:drawableLeft="@drawable/ic_print"
        android:drawableStart="@drawable/ic_print"
        android:text="@string/action_print"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView3"
        style="@style/ActionItem"
        />
</androidx.constraintlayout.widget.ConstraintLayout>
```
