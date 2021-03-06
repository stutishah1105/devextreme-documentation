Use the [columns](/Documentation/ApiReference/UI_Widgets/dxGantt/Configuration/#columns/) option to specify columns that the **Gantt** widget should display in the task list. The widget gets columns from the [tasks](/Documentation/ApiReference/UI_Widgets/dxGantt/Configuration/tasks/) data source.

    <!-- tab: index.js -->
    $(function() {
        $("#gantt").dxGantt({
            // ...
            columns: [{
                dataField: "title",
                caption: "Subject",
                width: 300
            }, {
                dataField: "start",
                caption: "Start Date"
            }, {
                dataField: "end",
                caption: "End Date"
            }],        
            ...
        });
    });
    
    <!-- tab: data.js -->
    var tasks = [{
        'id': 1,
        'parentId': 0,
        'title': 'Software Development',
        'start': new Date('2019-02-21T05:00:00.000Z'),
        'end': new Date('2019-07-04T12:00:00.000Z'),
        'progress': 31
    },      
        // ...
    ];
