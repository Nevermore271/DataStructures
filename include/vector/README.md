## Class vector

Class vector описывает объект - контейнер, представляющий последовательность для хранения элементов заданного типа в линейном порядке и быстрого произвольного доступа к любому из них. Он является наиболее подходящим типом контейнера для последовательности, когда на первом месте стоит производительность произвольного доступа.

https://msdn.microsoft.com/ru-ru/library/9xd04bzs.aspx

//уточнить про аллокатор и итератор

template <class Type, class Allocator = allocator<Type>>  
class vector

or

template <class Ty>
class vector

## Memebers

Ty* array_

size_t size_array

size_t count_

//...

## Methods

vector::assign	 Удаляет вектор и копирует указанные элементы в пустой вектор.

vector::at		 Возвращает ссылку на элемент в заданном положении в векторе.

vector::back	 Возвращает ссылку на последний элемент вектора.

vector::begin	 Возвращает итератор произвольного доступа, указывающий на первый элемент в векторе.

vector::capacity Возвращает число элементов, которое вектор может содержать без выделения дополнительного пространства.

vector::clear	 Очищает элементы вектора.

vector::data   	 Возвращает указатель на первый элемент в векторе.

vector::emplace	 Вставляет элемент, созданный на месте, в указанное положение в векторе.

vector::emplace_back	Добавляет элемент, созданный на месте, в конец вектора.

vector::empty	 Проверяет, пуст ли контейнер вектора.

vector::end   	 Возвращает итератор произвольного доступа, который указывает на конец вектора.

vector::erase	 Удаляет элемент или диапазон элементов в векторе из заданных позиций.

vector::front	 Возвращает ссылку на первый элемент в векторе.

vector::insert	 Вставляет элемент или некоторое число элементов в вектор в заданной позиции.

vector::max_size Возвращает максимальную длину вектора.

vector::pop_back Удаляет элемент в конце вектора.

vector::push_back Добавляет элемент в конец вектора.

vector::reserve	 Резервирует минимальную длину хранилища для объекта вектора.

vector::resize	 Определяет новый размер вектора.

vector::shrink_to_fit	Удаляет лишнюю емкость.

vector::size	 Возвращает количество элементов в векторе.

vector::swap	 Меняет местами элементы двух векторов.

//...

## Operators

vector::operator[]	Возвращает ссылку на элемент вектора в указанной позиции.

vector::operator =	Заменяет элементы вектора копией другого вектора.

//...

## OTHER

? vector::cbegin 	 Возвращает постоянный итератор произвольного доступа, указывающий на первый элемент в векторе.

? vector::cend	 Возвращает константный итератор произвольного доступа, указывающий на позицию, следующую за концом вектора.

? vector::crbegin	 Возвращает константный итератор, который указывает на первый элемент в обратном векторе.

? vector::crend	 Возвращает константный итератор, который указывает на последний элемент в обратном векторе.

? vector::get_allocator	Возвращает объект классу allocator, используемому вектором.

? vector::rbegin	 Возвращает итератор, указывающий на первый элемент в обратном векторе.

? vector::rend	 Возвращает итератор, который указывает на последний элемент в обратном векторе.

//...