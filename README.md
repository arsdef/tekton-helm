# tekton-helm
pipeline parametrizado de Tekton que genera un Helm chart 
Descripción del Pipeline:
Exportación de recursos: La primera tarea extrae todos los recursos relacionados con la aplicación desde Kubernetes (Deployment, Service, Ingress, ConfigMap, Secret, PVC).
Generación del Helm Chart: La segunda tarea crea el Helm chart y organiza los recursos dentro de la carpeta templates.
Subida a Git: La tercera tarea clona el repositorio Git, agrega los cambios, y realiza el push al repositorio.

Este pipeline es totalmente parametrizado, adaptable a diferentes aplicaciones, y asegura que todos los recursos estén correctamente organizados en un Helm chart.

EL fichero exportar_recursos.yaml es para kubernetes
El fichero exportar.openshift-recursos es para openshift 
