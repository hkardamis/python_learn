# python_learn

    Δημιουργήστε ένα νέο virtual environment
    C:\PythonProjects>virtualenv -p C:\python27\python.exe dvdstoreapp_venv

    Ενεργοποιήστε το virtual environment
   (dvdstoreapp_venv) C:\PythonProjects\dvdstoreapp_venv>scripts\activate.bat

    Εγκαταστήστε το django
    (dvdstoreapp_venv) C:\PythonProjects\dvdstoreapp_venv>pip install -U django

    Δημιουργήστε το django project dvdstore
    C:\PythonProjects\dvdstoreapp_venv>django-admin startproject dvdstore

    Εκκινήστε τον development server
    python manage.py runserver
	
	Δημιουργούμε ένα application με όνομα posts
    (dvdstoreapp_venv) C:\PythonProjects\dvdstoreapp_venv>cd dvdstore
    (dvdstoreapp_venv) C:\PythonProjects\dvdstoreapp_venv\dvdstore>python manage.py startapp dvdstore_app

	-->ΠΡΕΠΕΙ να πάω στο settings.py και να το δηλώσω στο  INSTALLED_APPS (να μη ξεχάσω το κόμμα στο τέλος .....)
	
	( δεν το έκανα ακόμα !!!!!!!!
	Για να εγκαταστήσουμε εφαρμογή
    pip install django-registration-redux
	)
	
	Για να δημιουργηθούν οι αντίστοιχοι πίνακες στην βάση κάνουμε migration:
	python manage.py makemigrations
	python manage.py migrate
		
	Δημιουργω superUser για το admin του Django (harris/iez48680)
	python manage.py createsuperuser
