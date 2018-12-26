# Описание интерфейса IFilial
Интерфейс предназначен для работы с методами класса Filial

## Реализация интерфейса
* + AddManagerFromFilial(FilialID : int, ManagerID : Int) : Bool функция добавляющая менеджера в филиал
* + AddSubjectPledgeFomFilial(FilialID : Int, Subject_pledgeID : Int) : Bool  функция добавляющая предмет залога в филиал
* + Delete(Id : Int) : Bool Функция удаляющая филиалы
* + GetAllContract(FilialID : Int) : List <[Contract](Contract.md)>  функция получающая список контарктов
* + GetAllFilial(sorting : string, sortingA : string, filtering : Reader, count : Int, page : Int) : List <[Filial](Filial.md)> функция получающая список филиалов
Параметры:
	* sortinig: string — отвечает, по какому полю будет сортироваться список;
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
	* filtering: string — отвечает за фильтрацию;
	* count: int — отвечает, сколько элементов необходимо показать;
	* page: int — отвечает, с какой страницы начинать поиск элементов.

* + GetAllManagers(FilialID : Int) : List <[Manager](Manager.md)> функция получающая список менеджеров
* + GetAllSubjectPledge(FilialID : int) : List <[Subject_pledge](Subject_pledge.md)> функция получающая список предметов залога
* + Save(Filial : Int) : Bool  функция, редактирующая данные о филиале.