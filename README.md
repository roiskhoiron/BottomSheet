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
#### Kode XML (activity_main.xml)
```xml
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity" >
    <Button
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginBottom="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginLeft="8dp"
        android:layout_marginRight="8dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="8dp"
        android:background="@color/colorAccent"
        android:onClick="showBottomSheet"
        android:padding="8dp"
        android:text="Show BottomSheet"
        android:textColor="#fff"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.4"
        />
    <TextView
        android:id="@+id/tvSelectedItem"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginEnd="8dp"
        android:layout_marginLeft="8dp"
        android:layout_marginRight="8dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="32dp"
        android:textSize="@dimen/text_size"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/button"
        tools:text="Selected Item"
        />
</androidx.constraintlayout.widget.ConstraintLayout>
```
