# <a name="outlook-extended-properties-overview"></a>Outlook の拡張プロパティの概要

拡張プロパティではカスタム データを格納することができます。特に Outlook MAPI プロパティが_まだ Microsoft Graph API のメタデータで公開されていない_場合に、拡張プロパティは、アプリがこれらのプロパティのカスタム データにアクセスするためのフォールバック メカニズムとして機能します。拡張プロパティの REST API を使用して、次のユーザー リソースにこのようなカスタム データを格納したり、取得したりできます。

- [message](../resources/message.md)
- [mailFolder](../resources/mailfolder.md)
- [event](../resources/event.md)
- [calendar](../resources/calendar.md)
- [contact](../resources/contact.md)
- [contactFolder](../resources/contactfolder.md) 

または、次の Office 365 グループ リソースとの間でもデータをやり取りできます。

- グループ [event](../resources/event.md)
- グループ [calendar](../resources/calendar.md)
- グループ [post](../resources/post.md) 

## <a name="use-extended-properties-or-open-extensions"></a>拡張プロパティとオープン拡張機能のどちらを使用するか

最も一般的なシナリオとして、オープン拡張機能 ([openTypeExtension](../resources/opentypeextension.md) で表される。旧称は Office 365 のデータ拡張機能) を使用して、リソース インスタンスのカスタム データをユーザーのメールボックスに格納したり、それらにアクセスしたりできます。拡張プロパティは、[Microsoft Graph API のメタデータ](http://developer.microsoft.com/en-us/graph/docs/overview/call_api)でまだ公開されていない Outlook MAPI プロパティのカスタム データにアクセスする必要がある場合にのみ使用します。 

## <a name="types-of-extended-properties"></a>拡張プロパティのタイプ

拡張プロパティに単一の値を保存するか、または (同じ型の) 複数の値を保存するかに応じて、拡張プロパティを [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md)、または [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) として作成できます。

これらのタイプはそれぞれ、**id** によってプロパティを識別し、データを **value** に格納します。 

**id** を使用して、特定のリソース インスタンスをその拡張プロパティと一緒に取得するか、単一の値の拡張プロパティでフィルターして、そのプロパティのすべてのインスタンスを取得できます。 

**注** REST API を使用して、1 つの呼び出しで特定のインスタンスのすべての拡張プロパティを取得することはできません。
  

### <a name="id-formats"></a>id の形式

単一値または複数値の拡張プロパティを作成する場合、文字列の名前または数値識別子のいずれか、および値の実際の型またはプロパティの値に基づき、2 つの形式のいずれかで **id** を指定できます。Sinceextended プロパティはほとんどの場合、Microsoft Graph API メタデータで公開されていない定義済みの MAPI プロパティと相互運用します。簡略化のため、選択する形式は、対応する MAPI プロパティが [MAPI プロパティの識別子](https://msdn.microsoft.com/en-us/library/office/cc815528.aspx)で文字列を使用しているか、数値を使用しているかを反映する必要があります。\[MS-OXPROPS\] Microsoft Corporation の「[Exchange Server Protocols Master Property List](https://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx)」(Exchange Server プロトコルのマスター プロパティ リスト) では、既存の MAPI プロパティへの拡張プロパティのマッピングに関する情報 (プロパティ識別子や GUID など) を検索できます。

**注** **id** に対して 1 つの形式を選択したら、その形式でのみ拡張プロパティにアクセスする必要があります。


**単一値の拡張プロパティに有効な id の形式**

|**形式**|**例**|**説明**|
|:---------|:----------|:--------------|
| "*{type} {guid} **Name** {name}*" | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | 属している名前空間 (GUID) と名前で、プロパティを識別します。         |
| "*{type} {guid} **Id** {id}*"     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | 属している名前空間 (GUID) と識別子で、プロパティを識別します。  |

**複数値の拡張プロパティに有効な id の形式**

|**形式**|**例**|**説明**|
|:---------|:----------|:--------------|
| "*{type} {guid} **Name** {name}*" | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | 名前空間 (GUID) と名前でプロパティを識別します。         |
| "*{type} {guid} **Id** {id}*"     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | 名前空間 (GUID) と識別子でプロパティを識別します。   |

### <a name="rest-api-operations"></a>REST API の操作
 
単一値の拡張プロパティの操作:

- [新規または既存のリソースのインスタンスに、拡張プロパティを作成します](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md)
- [`$expand` または `$filter` を使用し、拡張プロパティを含むリソース インスタンスを 1 つまたはコレクションで取得します](../api/singlevaluelegacyextendedproperty_get.md)

複数値の拡張プロパティの操作:

- [新規または既存のリソースのインスタンスに、拡張プロパティを作成します](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md)
- [`$expand` を使用して拡張プロパティを含むリソース インスタンスを取得します](../api/multivaluelegacyextendedproperty_get.md)

