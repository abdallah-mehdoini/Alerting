-- Créer une alerte pour l'erreur 823
USE msdb;
GO
EXEC sp_add_alert
    @name = N'Erreur 823 - I/O Disk',
    @message_id = 823,
    @severity = 0,
    @enabled = 1,
    @delay_between_responses = 0,
    @include_event_description_in = 1,
    @notification_message = N'Erreur 823 détectée : problème d’E/S disque.';
GO

-- Créer une alerte pour l'erreur 824
EXEC sp_add_alert
    @name = N'Erreur 824 - Corruption logique',
    @message_id = 824,
    @severity = 0,
    @enabled = 1,
    @delay_between_responses = 0,
    @include_event_description_in = 1,
    @notification_message = N'Erreur 824 détectée : corruption logique dans une page.';
GO

-- Créer une alerte pour l'erreur 825
EXEC sp_add_alert
    @name = N'Erreur 825 - Lecture répétée',
    @message_id = 825,
    @severity = 0,
    @enabled = 1,
    @delay_between_responses = 0,
    @include_event_description_in = 1,
    @notification_message = N'Erreur 825 détectée : lecture répétée d’une page, disque instable.';
GO
