# Описание интерфейса IClients
Интерфейс предназначен для работы с методами класса Clients

## Реализация интерфейса
* + Delete(ID : Int) : Bool Функция удаляет клиента
* + GetAllClients(sorting : string, sortingA : string, filtering : Reader, count : Int, page : Int) : List <[Client](Client.md)> Функция, возвращающая список клиентов
Параметры:
	* sortinig: string — отвечает, по какому полю будет сортироваться список;
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
	* filtering: string — отвечает за фильтрацию;
	* count: int — отвечает, сколько элементов необходимо показать;
	* page: int — отвечает, с какой страницы начинать поиск элементов.
* + GetAllContract(ClientID : Int) : List <[Contract](Contract.md)> Функция, возвращающая список договоров
* + GetAllSubjectPledge(ClientID : Int) : List <[Subject_pledge](Subject_pledge.md)> Функция, возвращающая список предметов залога
* + GetPayList(ClientID : Int) : List <[Pay](Pay.md)> Функция, возвращающая список платежей
* + Save(Client : Int) : Bool функция, редактирующая данные о договоре.