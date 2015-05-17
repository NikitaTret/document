Функция varargout = Никита (varargin) gui_Singleton = 1; gui_State = структура («gui_Name", mfilename, ... gui_Singleton ", gui_Singleton, ... gui_OpeningFcn",Nikita_OpeningFcn, ... gui_OutputFcn ",Nikita_OutputFcn, ... gui_LayoutFcn", [],. .. "gui_Callback", []); если Наргин && ischar (varargin {1}) = gui_State.gui_Callback str2func (varargin {1}); конец

если nargout [varargout {1: nargout}] = gui_mainfcn (gui_State, varargin {:}); еще gui_mainfcn (gui_State, varargin {:}); конец функции Nikita_OpeningFcn (hObject, данныеСобытия, ручки, varargin) handles.output = hObject; guidata (hObject, ручки);

Функция varargout = Nikita_OutputFcn (hObject, данныеСобытия, ручки)

varargout {1} = handles.output;

% Программирование выпадающего меню для первой матрицы,% определение количества строк. Функция popupmenu1_Callback (hObject, данныеСобытия, ручки) комплект (handles.uitable1 "Видимый", "на"); п = Get (hObject, 'значение'); Dat = нули (N + 1, N + 1); = TRUE (1, N + 2); комплект (handles.uitable1, «Данные», Дат "ColumnEditable",)

функционировать popupmenu1_CreateFcn (hObject, данныеСобытия, ручки)

если МНПК && IsEqual (получить (hObject "BackgroundColor '), получим (0,' defaultUicontrolBackgroundColor ')) установлен (hObject" BackgroundColor "," белый "); конец

% Определение количества столбцов для второй матрицы. Функция popupmenu3_Callback (hObject2, данныеСобытия, ручки) комплект (handles.uitable2 "Видимый", "на"); м = Get (hObject2, 'Значение'); Dat2 = нули (т + 1, т + 1); B = TRUE (1, М + 2); комплект (handles.uitable2, «Данные», dat2 "ColumnEditable ', В)

функционировать popupmenu3_CreateFcn (hObject2, данныеСобытия, ручки)

если МНПК && IsEqual (получить (hObject2 "BackgroundColor '), получим (0,' defaultUicontrolBackgroundColor ')) установлен (hObject" BackgroundColor "," белый "); конец

Произведение% функция pushbutton1_Callback (hObject, данныеСобытия, ручки)% п = получить (handles.popupmenu1, 'значение'); = Получить (handles.uitable1, «Данные»); B = получить (handles.uitable2, «Данные»); х = * B; комплект (handles.text4, 'Строка', num2str (х), «Видимый», «О»)

Сложение% pushbutton2. Функция pushbutton2_Callback (hObject, данныеСобытия, ручки)% п = получить (handles.popupmenu1, 'значение'); = Получить (handles.uitable1, «Данные»); B = получить (handles.uitable2, «Данные»); х = A + B; комплект (handles.text4, 'Строка', num2str (х), «Видимый», «О»)

Вычитание% pushbutton3. Функция pushbutton3_Callback (hObject, данныеСобытия, ручки)% п = получить (handles.popupmenu1, 'значение'); = Получить (handles.uitable1, «Данные»); B = получить (handles.uitable2, «Данные»); х = АВ; комплект (handles.text4, 'Строка', num2str (х), «Видимый», «О»)

Транспонирование% в pushbutton4. Функция pushbutton4_Callback (hObject, данныеСобытия, ручки)% п = получить (handles.popupmenu1, 'значение'); = Получить (handles.uitable1, «Данные»); х = '. комплект (handles.text4, 'Строка', num2str (х), «Видимый», «О»)

Обратная% pushbutton5. Функция pushbutton5_Callback (hObject, данныеСобытия, ручки)% п = получить (handles.popupmenu1, 'значение'); = Получить (handles.uitable1, «Данные»); х = INV (А); комплект (handles.text4, 'Строка', num2str (х), «Видимый», «О»)

