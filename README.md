

## ConstraintLayouts, LinearLayouts, RelativeLayouts   :hatched_chick:

:one:  **Constraint Layout**

    <?xml version="1.0" encoding="utf-8"?>  
	<androidx.constraintlayout.widget.ConstraintLayout 		
	xmlns:android="http://schemas.android.com/apk/res/android"  
	xmlns:app="http://schemas.android.com/apk/res-auto"  
	xmlns:tools="http://schemas.android.com/tools"  
	android:layout_width="match_parent"  
	android:layout_height="match_parent"  
	tools:context=".ConstraintActivity">  
  
	 <ImageView  android:id="@+id/imageView"  
	  android:layout_width="wrap_content"  
	  android:layout_height="wrap_content"  
	  android:layout_marginTop="124dp"  
	  app:layout_constraintEnd_toEndOf="parent"  
	  app:layout_constraintStart_toStartOf="parent"  
	  app:layout_constraintTop_toTopOf="parent"  
	  app:srcCompat="@drawable/soptlogo" />  
  
	 <EditText  android:id="@+id/editText"  
		  android:layout_width="0dp"  
		  android:layout_height="wrap_content"  
		  android:layout_marginStart="24dp"  
		  android:layout_marginTop="48dp"  
		  android:layout_marginEnd="24dp"  
		  android:ems="10"  
		  android:hint="이메일"  
		  android:inputType="textPersonName"  
		  app:layout_constraintEnd_toEndOf="parent"  
		  app:layout_constraintStart_toStartOf="parent"  
		  app:layout_constraintTop_toBottomOf="@+id/imageView" />  
  
		 <EditText  android:id="@+id/editText2"  
	  android:layout_width="0dp"  
	  android:layout_height="wrap_content"  
	  android:layout_marginTop="16dp"  
	  android:ems="10"  
	  android:hint="비밀번호"  
	  android:inputType="textPassword"  
	  app:layout_constraintEnd_toEndOf="@+id/editText"  
	  app:layout_constraintStart_toStartOf="@+id/editText"  
	  app:layout_constraintTop_toBottomOf="@+id/editText" />  
  
	 <Button  android:id="@+id/button"  
	  android:layout_width="0dp"  
	  android:layout_height="wrap_content"  
	  android:layout_marginTop="32dp"  
	  android:text="로그인"  
	  app:layout_constraintEnd_toEndOf="@+id/editText2"  
	  app:layout_constraintHorizontal_bias="0.461"  
	  app:layout_constraintStart_toStartOf="@+id/editText2"  
	  app:layout_constraintTop_toBottomOf="@+id/editText2" />  
  
	 <TextView  android:id="@+id/textView"  
	  android:layout_width="wrap_content"  
	  android:layout_height="wrap_content"  
	  android:layout_marginTop="24dp"  
	  android:text="아직 회원이 아니신가요?"  
	  app:layout_constraintEnd_toStartOf="@+id/textView2"  
	  app:layout_constraintHorizontal_bias="0.5"  
	  app:layout_constraintHorizontal_chainStyle="packed"  
	  app:layout_constraintStart_toStartOf="parent"  
	  app:layout_constraintTop_toBottomOf="@+id/button" />  
  
	 <TextView  android:id="@+id/textView2"  
	  android:layout_width="wrap_content"  
	  android:layout_height="wrap_content"  
	  android:layout_marginStart="8dp"  
	  android:text="회원가입하기"  
	  app:layout_constraintBottom_toBottomOf="@+id/textView"  
	  app:layout_constraintEnd_toEndOf="parent"  
	  app:layout_constraintHorizontal_bias="0.5"  
	  app:layout_constraintStart_toEndOf="@+id/textView"  
	  app:layout_constraintTop_toTopOf="@+id/textView" />  
		</androidx.constraintlayout.widget.ConstraintLayout>
:two: **LinearLayout**

    <?xml version="1.0" encoding="utf-8"?>  
	<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"  
	  xmlns:app="http://schemas.android.com/apk/res-auto"  
	  xmlns:tools="http://schemas.android.com/tools"  
	  android:layout_width="match_parent"  
	  android:layout_height="match_parent"  
	  android:orientation="vertical"  
	  tools:context=".LinearActivity">  
  
	 <ImageView  android:id="@+id/imageView"  
	  android:layout_width="wrap_content"  
	  android:layout_height="wrap_content"  
	  android:layout_marginTop="126dp"  
	  android:layout_gravity="center"  
	  app:srcCompat="@drawable/soptlogo" />  
  
	 <EditText  android:id="@+id/editText"  
	  android:layout_width="wrap_content"  
	  android:layout_height="wrap_content"  
	  android:layout_gravity="center"  
	  android:layout_marginStart="24dp"  
	  android:layout_marginTop="48dp"  
	  android:layout_marginEnd="24dp"  
	  android:ems="10"  
	  android:hint="이메일"  
	  android:inputType="textPersonName"  
	  app:layout_constraintTop_toBottomOf="@+id/imageView" />  
  
		 <EditText  android:id="@+id/editText2"  
	  android:layout_width="wrap_content"  
	  android:layout_height="wrap_content"  
	  android:layout_gravity="center"  
	  android:layout_marginTop="16dp"  
	  android:ems="10"  
	  android:hint="비밀번호"  
	  android:inputType="textPassword"  
	  app:layout_constraintTop_toBottomOf="@+id/editText" />  
  
	 <Button  android:id="@+id/button"  
	  android:layout_width="wrap_content"  
	  android:layout_height="wrap_content"  
	  android:layout_marginTop="8dp"  
	  android:layout_gravity="center"  
	  android:text="로그인"  
	  app:layout_constraintEnd_toEndOf="@+id/editText2"  
	  />  
  
	 <LinearLayout  android:layout_width="wrap_content"  
	  android:layout_height="wrap_content"  
	  android:orientation="horizontal"  
	  android:layout_gravity="center"  
	  >  
  
	 <TextView  android:id="@+id/textView"  
	  android:layout_width="wrap_content"  
	  android:layout_height="wrap_content"  
	  android:layout_gravity="center"  
	  android:text="아직 회원이 아니신가요?" />  
  
	 <TextView  android:id="@+id/textView2"  
	  android:layout_width="wrap_content"  
	  android:layout_height="wrap_content"  
	  android:layout_gravity="center"  
	  android:layout_marginLeft="8dp"  
	  android:text="회원가입하기"  
	  />   </LinearLayout>  </LinearLayout>
:three: **Relative Layout**

    <?xml version="1.0" encoding="utf-8"?>  
	<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"  
	  xmlns:app="http://schemas.android.com/apk/res-auto"  
	  xmlns:tools="http://schemas.android.com/tools"  
	  android:layout_width="match_parent"  
	  android:layout_height="match_parent"  
	  tools:context=".RelativeActivity">  
  
	 <ImageView  android:id="@+id/imageView"  
	  android:layout_width="wrap_content"  
	  android:layout_height="wrap_content"  
	  android:layout_marginTop="124dp"  
	  android:layout_centerHorizontal = "true"  
	  app:srcCompat="@drawable/soptlogo" />  
  
	 <EditText  android:id="@+id/editText"  
	  android:layout_width="match_parent"  
	  android:layout_height="wrap_content"  
	  android:hint="이메일"  
	  android:inputType="textPersonName"  
	  android:layout_marginHorizontal = "24dp"  
	  android:layout_below = "@+id/imageView"  
	  android:layout_marginTop="24dp" />  
	 <EditText  android:id="@+id/editText2"  
	  android:layout_width="match_parent"  
	  android:layout_height="wrap_content"  
	  android:hint="비밀번호"  
	  android:layout_marginHorizontal = "24dp"  
	  android:layout_below = "@+id/editText"  
	  android:layout_marginTop="24dp" />  
  
	 <Button  android:id="@+id/button"  
	  android:layout_width="match_parent"  
	  android:layout_height="wrap_content"  
	  android:layout_below="@+id/editText2"  
	  android:layout_marginHorizontal = "24dp"  
	  android:layout_marginTop="24dp"  
	  android:text="로그인" />  
  
	 <LinearLayout  android:layout_width="wrap_content"  
	  android:layout_height="wrap_content"  
	  android:layout_below= "@+id/button"  
	  android:layout_marginTop="32dp"  
	  android:layout_centerHorizontal="true"  
	  android:orientation="horizontal">  
  
	 <TextView  android:id="@+id/textView"  
	  android:layout_width="wrap_content"  
	  android:layout_height="wrap_content"  
	  android:layout_marginTop="2dp"  
	  android:text="아직 회원이 아니신가요?" />  
	  
	 <TextView  android:id="@+id/textView2"  
	  android:layout_width="wrap_content"  
	  android:layout_height="wrap_content"  
	  android:layout_marginLeft="8dp"  
	  android:text="회원가입하기"></TextView>  
	 </LinearLayout>  
  
	</RelativeLayout>
