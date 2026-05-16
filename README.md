Execution log:

<img width="1698" height="748" alt="image" src="https://github.com/user-attachments/assets/c0c9f3c7-dd23-43f4-9186-82ed680a911e" />

***
"C:\Program Files\Java\jdk-21\bin\java.exe" "-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA 2026.1.1\lib\idea_rt.jar=61240" -Dfile.encoding=UTF-8 -Dsun.stdout.encoding=UTF-8 -Dsun.stderr.encoding=UTF-8 -classpath C:\Users\isalm\IdeaProjects\TP4\target\classes;C:\Users\isalm\.m2\repository\javax\persistence\javax.persistence-api\2.2\javax.persistence-api-2.2.jar;C:\Users\isalm\.m2\repository\org\hibernate\hibernate-core\5.6.5.Final\hibernate-core-5.6.5.Final.jar;C:\Users\isalm\.m2\repository\org\jboss\logging\jboss-logging\3.4.3.Final\jboss-logging-3.4.3.Final.jar;C:\Users\isalm\.m2\repository\net\bytebuddy\byte-buddy\1.12.7\byte-buddy-1.12.7.jar;C:\Users\isalm\.m2\repository\antlr\antlr\2.7.7\antlr-2.7.7.jar;C:\Users\isalm\.m2\repository\org\jboss\spec\javax\transaction\jboss-transaction-api_1.2_spec\1.1.1.Final\jboss-transaction-api_1.2_spec-1.1.1.Final.jar;C:\Users\isalm\.m2\repository\org\jboss\jandex\2.4.2.Final\jandex-2.4.2.Final.jar;C:\Users\isalm\.m2\repository\com\fasterxml\classmate\1.5.1\classmate-1.5.1.jar;C:\Users\isalm\.m2\repository\javax\activation\javax.activation-api\1.2.0\javax.activation-api-1.2.0.jar;C:\Users\isalm\.m2\repository\org\hibernate\common\hibernate-commons-annotations\5.1.2.Final\hibernate-commons-annotations-5.1.2.Final.jar;C:\Users\isalm\.m2\repository\javax\xml\bind\jaxb-api\2.3.1\jaxb-api-2.3.1.jar;C:\Users\isalm\.m2\repository\org\glassfish\jaxb\jaxb-runtime\2.3.1\jaxb-runtime-2.3.1.jar;C:\Users\isalm\.m2\repository\org\glassfish\jaxb\txw2\2.3.1\txw2-2.3.1.jar;C:\Users\isalm\.m2\repository\com\sun\istack\istack-commons-runtime\3.0.7\istack-commons-runtime-3.0.7.jar;C:\Users\isalm\.m2\repository\org\jvnet\staxex\stax-ex\1.8\stax-ex-1.8.jar;C:\Users\isalm\.m2\repository\com\sun\xml\fastinfoset\FastInfoset\1.2.15\FastInfoset-1.2.15.jar;C:\Users\isalm\.m2\repository\org\hibernate\validator\hibernate-validator\6.2.0.Final\hibernate-validator-6.2.0.Final.jar;C:\Users\isalm\.m2\repository\jakarta\validation\jakarta.validation-api\2.0.2\jakarta.validation-api-2.0.2.jar;C:\Users\isalm\.m2\repository\com\h2database\h2\2.1.214\h2-2.1.214.jar;C:\Users\isalm\.m2\repository\org\slf4j\slf4j-api\1.7.36\slf4j-api-1.7.36.jar;C:\Users\isalm\.m2\repository\org\slf4j\slf4j-simple\1.7.36\slf4j-simple-1.7.36.jar org.example.App
May 16, 2026 3:25:36 AM org.hibernate.jpa.internal.util.LogHelper logPersistenceUnitInformation
INFO: HHH000204: Processing PersistenceUnitInfo [name: hibernate-inheritance]
May 16, 2026 3:25:36 AM org.hibernate.Version logVersion
INFO: HHH000412: Hibernate ORM core version 5.6.5.Final
May 16, 2026 3:25:37 AM org.hibernate.annotations.common.reflection.java.JavaReflectionManager <clinit>
INFO: HCANN000001: Hibernate Commons Annotations {5.1.2.Final}
May 16, 2026 3:25:37 AM org.hibernate.engine.jdbc.connections.internal.DriverManagerConnectionProviderImpl configure
WARN: HHH10001002: Using Hibernate built-in connection pool (not for production use!)
May 16, 2026 3:25:37 AM org.hibernate.engine.jdbc.connections.internal.DriverManagerConnectionProviderImpl buildCreator
INFO: HHH10001005: using driver [org.h2.Driver] at URL [jdbc:h2:mem:testdb;DB_CLOSE_DELAY=-1]
May 16, 2026 3:25:37 AM org.hibernate.engine.jdbc.connections.internal.DriverManagerConnectionProviderImpl buildCreator
INFO: HHH10001001: Connection properties: {password=****, user=sa}
May 16, 2026 3:25:37 AM org.hibernate.engine.jdbc.connections.internal.DriverManagerConnectionProviderImpl buildCreator
INFO: HHH10001003: Autocommit mode: false
May 16, 2026 3:25:37 AM org.hibernate.engine.jdbc.connections.internal.DriverManagerConnectionProviderImpl$PooledConnections <init>
INFO: HHH000115: Hibernate connection pool size: 20 (min=1)
May 16, 2026 3:25:37 AM org.hibernate.dialect.Dialect <init>
INFO: HHH000400: Using dialect: org.hibernate.dialect.H2Dialect
May 16, 2026 3:25:38 AM org.hibernate.validator.internal.util.Version <clinit>
INFO: HV000001: Hibernate Validator 6.2.0.Final
May 16, 2026 3:25:39 AM org.hibernate.resource.transaction.backend.jdbc.internal.DdlTransactionIsolatorNonJtaImpl getIsolatedConnection
INFO: HHH10001501: Connection obtained from JdbcConnectionAccess [org.hibernate.engine.jdbc.env.internal.JdbcEnvironmentInitiator$ConnectionProviderJdbcConnectionAccess@4bd51d3e] for (non-JTA) DDL execution was not in auto-commit mode; the Connection 'local transaction' will be committed and the Connection will be set into auto-commit mode.
Hibernate: 
    
    create table developpeurs (
       anneeExperience integer,
        langage varchar(255),
        specialite varchar(255),
        id bigint not null,
        primary key (id)
    )
Hibernate: 
    
    create table electroniques (
       id bigint not null,
        dateCreation timestamp,
        description varchar(255),
        nom varchar(255),
        prix double,
        caracteristiques varchar(255),
        garantieMois integer,
        marque varchar(255),
        modele varchar(255),
        primary key (id)
    )
Hibernate: 
    
    create table employes (
       id bigint generated by default as identity,
        dateEmbauche date,
        email varchar(255),
        nom varchar(255),
        prenom varchar(255),
        primary key (id)
    )
Hibernate: 
    
    create table livres (
       id bigint not null,
        dateCreation timestamp,
        description varchar(255),
        nom varchar(255),
        prix double,
        auteur varchar(255),
        editeur varchar(255),
        isbn varchar(255),
        nombrePages integer,
        primary key (id)
    )
Hibernate: 
    
    create table managers (
       bonus double,
        nombreSubordonnes integer,
        service varchar(255),
        id bigint not null,
        primary key (id)
    )
Hibernate: 
    
    create table vehicules (
       type_vehicule varchar(31) not null,
        id bigint generated by default as identity,
        anneeFabrication date,
        marque varchar(255),
        modele varchar(255),
        prix double,
        climatisation boolean,
        nombrePortes integer,
        typeCarburant varchar(255),
        cylindree integer,
        typeTransmission varchar(255),
        primary key (id)
    )
Hibernate: create sequence hibernate_sequence start with 1 increment by 1
Hibernate: 
    
    alter table developpeurs 
       add constraint FK9j5p325r527m0cjurrle82v55 
       foreign key (id) 
       references employes
Hibernate: 
    
    alter table managers 
       add constraint FKr9ijmk08aebix1ncjqa4y1k69 
       foreign key (id) 
       references employes
May 16, 2026 3:25:39 AM org.hibernate.engine.transaction.jta.platform.internal.JtaPlatformInitiator initiateService
INFO: HHH000490: Using JtaPlatform implementation: [org.hibernate.engine.transaction.jta.platform.internal.NoJtaPlatform]

=== Test de la stratégie SINGLE_TABLE ===
Création des véhicules...
Hibernate: 
    insert 
    into
        vehicules
        (id, anneeFabrication, marque, modele, prix, climatisation, nombrePortes, typeCarburant, type_vehicule) 
    values
        (default, ?, ?, ?, ?, ?, ?, ?, 'VOITURE')
Hibernate: 
    insert 
    into
        vehicules
        (id, anneeFabrication, marque, modele, prix, climatisation, nombrePortes, typeCarburant, type_vehicule) 
    values
        (default, ?, ?, ?, ?, ?, ?, ?, 'VOITURE')
Hibernate: 
    insert 
    into
        vehicules
        (id, anneeFabrication, marque, modele, prix, cylindree, typeTransmission, type_vehicule) 
    values
        (default, ?, ?, ?, ?, ?, ?, 'MOTO')
Véhicules créés avec succès !

Récupération de tous les véhicules :
Hibernate: 
    select
        vehicule0_.id as id2_6_,
        vehicule0_.anneeFabrication as anneefab3_6_,
        vehicule0_.marque as marque4_6_,
        vehicule0_.modele as modele5_6_,
        vehicule0_.prix as prix6_6_,
        vehicule0_.climatisation as climatis7_6_,
        vehicule0_.nombrePortes as nombrepo8_6_,
        vehicule0_.typeCarburant as typecarb9_6_,
        vehicule0_.cylindree as cylindr10_6_,
        vehicule0_.typeTransmission as typetra11_6_,
        vehicule0_.type_vehicule as type_veh1_6_ 
    from
        vehicules vehicule0_
Voiture{id=1, marque='Renault', modele='Clio', anneeFabrication=2020-05-15, prix=15000.0, nombrePortes=5, climatisation=true, typeCarburant='Essence'}
Voiture{id=2, marque='Peugeot', modele='308', anneeFabrication=2019-03-10, prix=18000.0, nombrePortes=5, climatisation=true, typeCarburant='Diesel'}
Moto{id=3, marque='Honda', modele='CBR', anneeFabrication=2021-07-20, prix=12000.0, cylindree=600, typeTransmission='Manuelle'}

Récupération de toutes les voitures :
Hibernate: 
    select
        voiture0_.id as id2_6_,
        voiture0_.anneeFabrication as anneefab3_6_,
        voiture0_.marque as marque4_6_,
        voiture0_.modele as modele5_6_,
        voiture0_.prix as prix6_6_,
        voiture0_.climatisation as climatis7_6_,
        voiture0_.nombrePortes as nombrepo8_6_,
        voiture0_.typeCarburant as typecarb9_6_ 
    from
        vehicules voiture0_ 
    where
        voiture0_.type_vehicule='VOITURE'
Voiture{id=1, marque='Renault', modele='Clio', anneeFabrication=2020-05-15, prix=15000.0, nombrePortes=5, climatisation=true, typeCarburant='Essence'}
Voiture{id=2, marque='Peugeot', modele='308', anneeFabrication=2019-03-10, prix=18000.0, nombrePortes=5, climatisation=true, typeCarburant='Diesel'}

Récupération de toutes les motos :
Hibernate: 
    select
        moto0_.id as id2_6_,
        moto0_.anneeFabrication as anneefab3_6_,
        moto0_.marque as marque4_6_,
        moto0_.modele as modele5_6_,
        moto0_.prix as prix6_6_,
        moto0_.cylindree as cylindr10_6_,
        moto0_.typeTransmission as typetra11_6_ 
    from
        vehicules moto0_ 
    where
        moto0_.type_vehicule='MOTO'
Moto{id=3, marque='Honda', modele='CBR', anneeFabrication=2021-07-20, prix=12000.0, cylindree=600, typeTransmission='Manuelle'}

=== Test de la stratégie JOINED ===
Création des employés...
Hibernate: 
    insert 
    into
        employes
        (id, dateEmbauche, email, nom, prenom) 
    values
        (default, ?, ?, ?, ?)
Hibernate: 
    insert 
    into
        developpeurs
        (anneeExperience, langage, specialite, id) 
    values
        (?, ?, ?, ?)
Hibernate: 
    insert 
    into
        employes
        (id, dateEmbauche, email, nom, prenom) 
    values
        (default, ?, ?, ?, ?)
Hibernate: 
    insert 
    into
        developpeurs
        (anneeExperience, langage, specialite, id) 
    values
        (?, ?, ?, ?)
Hibernate: 
    insert 
    into
        employes
        (id, dateEmbauche, email, nom, prenom) 
    values
        (default, ?, ?, ?, ?)
Hibernate: 
    insert 
    into
        managers
        (bonus, nombreSubordonnes, service, id) 
    values
        (?, ?, ?, ?)
Employés créés avec succès !

Récupération de tous les employés :
Hibernate: 
    select
        employe0_.id as id1_2_,
        employe0_.dateEmbauche as dateemba2_2_,
        employe0_.email as email3_2_,
        employe0_.nom as nom4_2_,
        employe0_.prenom as prenom5_2_,
        employe0_1_.anneeExperience as anneeexp1_0_,
        employe0_1_.langage as langage2_0_,
        employe0_1_.specialite as speciali3_0_,
        employe0_2_.bonus as bonus1_4_,
        employe0_2_.nombreSubordonnes as nombresu2_4_,
        employe0_2_.service as service3_4_,
        case 
            when employe0_1_.id is not null then 1 
            when employe0_2_.id is not null then 2 
            when employe0_.id is not null then 0 
        end as clazz_ 
    from
        employes employe0_ 
    left outer join
        developpeurs employe0_1_ 
            on employe0_.id=employe0_1_.id 
    left outer join
        managers employe0_2_ 
            on employe0_.id=employe0_2_.id
Developpeur{id=1, nom='Dupont', prenom='Jean', email='jean.dupont@example.com', dateEmbauche=2019-05-15, langage='Java', specialite='Backend', anneeExperience=5}
Developpeur{id=2, nom='Martin', prenom='Sophie', email='sophie.martin@example.com', dateEmbauche=2020-03-10, langage='JavaScript', specialite='Frontend', anneeExperience=3}
Manager{id=3, nom='Dubois', prenom='Pierre', email='pierre.dubois@example.com', dateEmbauche=2018-07-20, service='IT', nombreSubordonnes=10, bonus=5000.0}

Récupération de tous les développeurs :
Hibernate: 
    select
        developpeu0_.id as id1_2_,
        developpeu0_1_.dateEmbauche as dateemba2_2_,
        developpeu0_1_.email as email3_2_,
        developpeu0_1_.nom as nom4_2_,
        developpeu0_1_.prenom as prenom5_2_,
        developpeu0_.anneeExperience as anneeexp1_0_,
        developpeu0_.langage as langage2_0_,
        developpeu0_.specialite as speciali3_0_ 
    from
        developpeurs developpeu0_ 
    inner join
        employes developpeu0_1_ 
            on developpeu0_.id=developpeu0_1_.id
Developpeur{id=1, nom='Dupont', prenom='Jean', email='jean.dupont@example.com', dateEmbauche=2019-05-15, langage='Java', specialite='Backend', anneeExperience=5}
Developpeur{id=2, nom='Martin', prenom='Sophie', email='sophie.martin@example.com', dateEmbauche=2020-03-10, langage='JavaScript', specialite='Frontend', anneeExperience=3}

Récupération de tous les managers :
Hibernate: 
    select
        manager0_.id as id1_2_,
        manager0_1_.dateEmbauche as dateemba2_2_,
        manager0_1_.email as email3_2_,
        manager0_1_.nom as nom4_2_,
        manager0_1_.prenom as prenom5_2_,
        manager0_.bonus as bonus1_4_,
        manager0_.nombreSubordonnes as nombresu2_4_,
        manager0_.service as service3_4_ 
    from
        managers manager0_ 
    inner join
        employes manager0_1_ 
            on manager0_.id=manager0_1_.id
Manager{id=3, nom='Dubois', prenom='Pierre', email='pierre.dubois@example.com', dateEmbauche=2018-07-20, service='IT', nombreSubordonnes=10, bonus=5000.0}

=== Test de la stratégie TABLE_PER_CLASS ===
Création des produits...
Hibernate: 
    call next value for hibernate_sequence
Hibernate: 
    call next value for hibernate_sequence
Hibernate: 
    call next value for hibernate_sequence
Hibernate: 
    insert 
    into
        livres
        (dateCreation, description, nom, prix, auteur, editeur, isbn, nombrePages, id) 
    values
        (?, ?, ?, ?, ?, ?, ?, ?, ?)
Hibernate: 
    insert 
    into
        livres
        (dateCreation, description, nom, prix, auteur, editeur, isbn, nombrePages, id) 
    values
        (?, ?, ?, ?, ?, ?, ?, ?, ?)
Hibernate: 
    insert 
    into
        electroniques
        (dateCreation, description, nom, prix, caracteristiques, garantieMois, marque, modele, id) 
    values
        (?, ?, ?, ?, ?, ?, ?, ?, ?)
Produits créés avec succès !

Récupération de tous les produits :
Hibernate: 
    select
        produit0_.id as id1_5_,
        produit0_.dateCreation as datecrea2_5_,
        produit0_.description as descript3_5_,
        produit0_.nom as nom4_5_,
        produit0_.prix as prix5_5_,
        produit0_.auteur as auteur1_3_,
        produit0_.editeur as editeur2_3_,
        produit0_.isbn as isbn3_3_,
        produit0_.nombrePages as nombrepa4_3_,
        produit0_.caracteristiques as caracter1_1_,
        produit0_.garantieMois as garantie2_1_,
        produit0_.marque as marque3_1_,
        produit0_.modele as modele4_1_,
        produit0_.clazz_ as clazz_ 
    from
        ( select
            id,
            dateCreation,
            description,
            nom,
            prix,
            auteur,
            editeur,
            isbn,
            nombrePages,
            null as caracteristiques,
            null as garantieMois,
            null as marque,
            null as modele,
            1 as clazz_ 
        from
            livres 
        union
        all select
            id,
            dateCreation,
            description,
            nom,
            prix,
            null as auteur,
            null as editeur,
            null as isbn,
            null as nombrePages,
            caracteristiques,
            garantieMois,
            marque,
            modele,
            2 as clazz_ 
        from
            electroniques 
    ) produit0_
Livre{id=1, nom='Le Seigneur des Anneaux', prix=25.99, description='Un classique de fantasy', dateCreation=2026-05-16T03:25:39.721915, auteur='J.R.R. Tolkien', isbn='978-2075134729', nombrePages=1200, editeur='Pocket'}
Livre{id=2, nom='Harry Potter', prix=19.99, description='Roman fantastique pour jeunes', dateCreation=2026-05-16T03:25:39.721915, auteur='J.K. Rowling', isbn='978-2070643028', nombrePages=800, editeur='Gallimard'}
Electronique{id=3, nom='Smartphone Galaxy S21', prix=899.99, description='Smartphone haut de gamme', dateCreation=2026-05-16T03:25:39.721915, marque='Samsung', modele='S21', garantieMois=24, caracteristiques='Écran 6.2", 128Go, 8Go RAM'}

Récupération de tous les livres :
Hibernate: 
    select
        livre0_.id as id1_5_,
        livre0_.dateCreation as datecrea2_5_,
        livre0_.description as descript3_5_,
        livre0_.nom as nom4_5_,
        livre0_.prix as prix5_5_,
        livre0_.auteur as auteur1_3_,
        livre0_.editeur as editeur2_3_,
        livre0_.isbn as isbn3_3_,
        livre0_.nombrePages as nombrepa4_3_ 
    from
        livres livre0_
Livre{id=1, nom='Le Seigneur des Anneaux', prix=25.99, description='Un classique de fantasy', dateCreation=2026-05-16T03:25:39.721915, auteur='J.R.R. Tolkien', isbn='978-2075134729', nombrePages=1200, editeur='Pocket'}
Livre{id=2, nom='Harry Potter', prix=19.99, description='Roman fantastique pour jeunes', dateCreation=2026-05-16T03:25:39.721915, auteur='J.K. Rowling', isbn='978-2070643028', nombrePages=800, editeur='Gallimard'}

Récupération de tous les produits électroniques :
Hibernate: 
    select
        electroniq0_.id as id1_5_,
        electroniq0_.dateCreation as datecrea2_5_,
        electroniq0_.description as descript3_5_,
        electroniq0_.nom as nom4_5_,
        electroniq0_.prix as prix5_5_,
        electroniq0_.caracteristiques as caracter1_1_,
        electroniq0_.garantieMois as garantie2_1_,
        electroniq0_.marque as marque3_1_,
        electroniq0_.modele as modele4_1_ 
    from
        electroniques electroniq0_
Electronique{id=3, nom='Smartphone Galaxy S21', prix=899.99, description='Smartphone haut de gamme', dateCreation=2026-05-16T03:25:39.721915, marque='Samsung', modele='S21', garantieMois=24, caracteristiques='Écran 6.2", 128Go, 8Go RAM'}
May 16, 2026 3:25:39 AM org.hibernate.engine.jdbc.connections.internal.DriverManagerConnectionProviderImpl$PoolState stop
INFO: HHH10001008: Cleaning up connection pool [jdbc:h2:mem:testdb;DB_CLOSE_DELAY=-1]

Process finished with exit code 0

***

<img width="1845" height="915" alt="image" src="https://github.com/user-attachments/assets/725d6604-784d-4e11-b494-4c46828a68d3" />
