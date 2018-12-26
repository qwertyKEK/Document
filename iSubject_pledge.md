# Описание интерфейса ISubject_pledge
Интерфейс предназначен для работы с методами класса Subject_pledge

## Реализация интерфейса
* + Add (Subject_pledge: [Subject_pledge](Subject_pledge.md)): Int — функция, добавляющая предмет залога в базу данных.
* + Delete(Id : Int) : Bool Функция удаляющая предметы залога
* + FindBySubject_pledgeNum(Subject_pledgeID : int) : [Subject_pledge](Subject_pledge.md)  функция, осуществляющая поиск предмета залога в базе данных по ID и возвращающая найденный, если такой есть.
* + FindByTitle(title_Subject_pledge : string) : [Subject_pledge](Subject_pledge.md)  функция, осуществляющая поиск платежа в базе данных по названию.
* + GetAllSubjectPledge(sorting : string, sortingA : string, filtering : Reader, count : Int, page : Int) : List<[Subject_pledge](Subject_pledge.md)> функция получающая список предметов залога
Параметры:
	* sortinig: string — отвечает, по какому полю будет сортироваться список;
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
	* filtering: string — отвечает за фильтрацию;
	* count: int — отвечает, сколько элементов необходимо показать;
	* page: int — отвечает, с какой страницы начинать поиск элементов.

* + GetStatus(Subject_pledge_ID : string) : [Subject_pledge](Subject_pledge.md)
* + Save(Subject_pledge : [Subject_pledge](Subject_pledge.md)) : Bool функция, редактирующая данные о предмете залога.