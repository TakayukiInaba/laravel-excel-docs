# Export concerns

| Interface | Explanation | Documentation |
|---- |----|----|
|`Maatwebsite\Excel\Concerns\FromArray`| Use an array to populate the export. | |
|`Maatwebsite\Excel\Concerns\FromCollection`| Use a Laravel Collection to populate the export. | [Exporting collections](/3.1/exports/collection.html) |
|`Maatwebsite\Excel\Concerns\FromIterator`| Use an iterator to populate the export. | |
|`Maatwebsite\Excel\Concerns\FromQuery`| Use an Eloquent query to populate the export. | [From Query](/3.1/exports/from-query.html) | 
|`Maatwebsite\Excel\Concerns\FromView`| Use a (Blade) view to to populate the export. | [From View](/3.1/exports/from-view.html) |
|`Maatwebsite\Excel\Concerns\WithTitle`| Set the Workbook or Worksheet title. | [Multiple Sheets](/3.1/exports/multiple-sheets.html) |
|`Maatwebsite\Excel\Concerns\WithHeadings`| Prepend a heading row. | [Adding a heading row](/3.1/exports/mapping.html#adding-a-heading-row) |
|`Maatwebsite\Excel\Concerns\WithMapping`| Format the row before it's written to the file. | [Mapping data](/3.1/exports/mapping.html) |
|`Maatwebsite\Excel\Concerns\WithColumnFormatting`| Format certain columns. | [Formatting columns](/3.1/exports/column-formatting.html) |
|`Maatwebsite\Excel\Concerns\WithMultipleSheets`| Enable multi-sheet support. Each sheet can have its own concerns (except this one). | [Multiple Sheets](/3.1/exports/multiple-sheets.html) |
|`Maatwebsite\Excel\Concerns\ShouldAutoSize`| Auto-size the columns in the worksheet. | [Auto size](/3.1/exports/column-formatting.html#auto-size) |
|`Maatwebsite\Excel\Concerns\WithStrictNullComparison`| Uses strict comparisions when testing cells for null value. | [Strict null comparisons](/3.1/exports/collection.html#strict-null-comparisons) |
|`Maatwebsite\Excel\Concerns\WithEvents`| Register events to hook into the PhpSpreadsheet process. | [Events](/3.1/exports/extending.html#events) |
|`Maatwebsite\Excel\Concerns\WithCustomQuerySize`| Allows Exportables that implement the FromQuery concern, to provide their own custom query size. | |
|`Maatwebsite\Excel\Concerns\WithCustomCsvSettings`| Allows to run custom Csv settings for this specific exportable. | [Custom CSV Settings](/3.1/imports/custom-csv-settings.html) |
|`Maatwebsite\Excel\Concerns\WithCharts`| Allows to run one or multiple PhpSpreadsheet Chart instances. | |
|`Maatwebsite\Excel\Concerns\WithDrawings`| Allows to run one or multiple PhpSpreadsheet (Base)Drawing instances. | |
|`Maatwebsite\Excel\Concerns\WithCustomStartCell`| Allows to specify a custom start cell. Do note that this is only supported for FromCollection exports. | |

### Traits

| Trait | Explanation | Documentation |
|---- |----|----|
|`Maatwebsite\Excel\Concerns\Exportable` | Add download/store abilities right on the export class itself. | [Exportables](/3.1/exports/exportables.html) |
|`Maatwebsite\Excel\Concerns\RegistersEventListeners` | Auto-register the available event listeners. | [Auto register event listeners](/3.1/exports/extending.html#auto-register-event-listeners) |
