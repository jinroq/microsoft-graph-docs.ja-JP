---
title: Outlook の拡張プロパティの概要
description: '拡張プロパティは、カスタム データを格納できるようにして、アプリケーションにアクセスするためのフォールバック メカニズムとしてサービスの提供に '
ms.openlocfilehash: a15c44c832971d0fc91cd1cc9e9c29db80715130
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071467"
---
# <a name="outlook-extended-properties-overview"></a>Outlook の拡張プロパティの概要

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

拡張プロパティではカスタム データを格納することができます。特に Outlook MAPI プロパティが_まだ Microsoft Graph API のメタデータで公開されていない_場合に、拡張プロパティは、アプリがこれらのプロパティのカスタム データにアクセスするためのフォールバック メカニズムとして機能します。拡張プロパティの REST API を使用して、次のユーザー リソースにこのようなカスタム データを格納したり、取得したりできます。

- [message](../resources/message.md)
- [mailFolder](../resources/mailfolder.md)
- [event](../resources/event.md)
- [calendar](../resources/calendar.md)
- [contact](../resources/contact.md)
- [contactFolder](../resources/contactfolder.md)
- [Outlook タスク](../resources/outlooktask.md)
- [Outlook の仕事フォルダー](../resources/outlooktaskfolder.md) 

または、次の Office 365 グループ リソースとの間でもデータをやり取りできます。

- グループ [event](../resources/event.md)
- グループ [calendar](../resources/calendar.md)
- グループ [post](../resources/post.md) 

## <a name="use-extended-properties-or-open-extensions"></a>拡張プロパティとオープン拡張機能のどちらを使用するか

最も一般的なシナリオとして、オープン拡張機能 ([openTypeExtension](../resources/opentypeextension.md) で表される。旧称は Office 365 のデータ拡張機能) を使用して、リソース インスタンスのカスタム データをユーザーのメールボックスに格納したり、それらにアクセスしたりできます。拡張プロパティは、[Microsoft Graph API のメタデータ](https://developer.microsoft.com/graph/docs/overview/call_api)でまだ公開されていない Outlook MAPI プロパティのカスタム データにアクセスする必要がある場合にのみ使用します。

## <a name="types-of-extended-properties"></a>拡張プロパティのタイプ

拡張プロパティに単一の値を保存するか、または (同じ型の) 複数の値を保存するかに応じて、拡張プロパティを [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)、または [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) として作成できます。

これらのタイプはそれぞれ、**id** によってプロパティを識別し、データを **value** に格納します。 

**id** を使用して、特定のリソース インスタンスをその拡張プロパティと一緒に取得するか、単一の値の拡張プロパティでフィルターして、そのプロパティのすべてのインスタンスを取得できます。 

**注** REST API を使用して、1 つの呼び出しで特定のインスタンスのすべての拡張プロパティを取得することはできません。
  

### <a name="id-formats"></a>id の形式

3 つの形式のいずれかでは、拡張プロパティの**id**を指定できます。

- 名前付きプロパティとして、拡張プロパティの型、名前空間、および文字列名によって識別します。
- 名前付きプロパティとして、拡張プロパティの型、名前空間、および数値識別子によって識別されます。
- Proptag の形式で、拡張プロパティの型、および[MAPI プロパティ タグ](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags)で識別されます。

次の 2 つのテーブルは、単一および複数の値に適用されている拡張プロパティとして、これらの形式を記述します。 {_タイプ_} では、拡張プロパティの値の種類を表します。 この例では、文字列、整数、およびこれらの種類の配列を示しています。

**単一値の拡張プロパティに有効な id の形式**

|**形式**|**例**|**説明**|
|:---------|:----------|:--------------|
| "{_type_} {_guid_} **Name** {_name_}" | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | それが属している名前空間 (GUID) と文字列名によってプロパティを識別します。         |
| "{_type_} {_guid_} **Id** {_id_}"     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | プロパティが属している名前空間 (GUID) と数値の識別子を指定します。  |
| [{_タイプ_} {_proptag_}]                    | ```"String 0x4001001E"```                                           | プロパティ タグを事前に定義されたプロパティを識別します。 |

**複数値の拡張プロパティに有効な id の形式**

|**形式**|**例**|**説明**|
|:---------|:----------|:--------------|
| "{_type_} {_guid_} **Name** {_name_}" | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | 名前空間 (GUID) と文字列名によってプロパティを識別します。         |
| "{_type_} {_guid_} **Id** {_id_}"     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | 数値識別子 (GUID) の名前空間によってプロパティを識別します。   |
| [{_タイプ_} {_proptag_}]                    | ```"StringArray 0x4002101E"```                                           | プロパティ タグを事前に定義されたプロパティを識別します。 |


単一値または複数値の拡張プロパティをカスタム プロパティとして定義するのにには、名前付きプロパティの形式のいずれかを使用します。 2 つの形式では、文字列の名前 (**名**) は、1 つ目は参照の容易にするために優先されるフォーマットがあります。 名前付きプロパティでは、その[プロパティの識別子](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview)を持つ 0x8000-0 xfffe の範囲です。

Proptag 形式を使用して、MAPI、または、クライアントまたはサーバーで定義済みのプロパティにアクセスしてするが既に公開されていない Microsoft Graph で。 これらのプロパティでは、プロパティの識別子を持つ、0x0001 0x7fff の範囲です。 Proptag 形式を使用してカスタム プロパティを定義しないでください。 


  \[MS-OXPROPS\] Microsoft Corporation の[「Exchange Server プロトコルのマスター プロパティ リスト」](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx)では、既存の MAPI プロパティへの拡張プロパティのマッピングに関する情報 (プロパティ識別子や GUID など) を検索できます。

**注** **id** に対して 1 つの形式を選択したら、その形式でのみ拡張プロパティにアクセスする必要があります。

## <a name="rest-api-operations"></a>REST API の操作
 
単一値の拡張プロパティの操作:

- [新規または既存のリソースのインスタンスに、拡張プロパティを作成します](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [`$expand` または `$filter` を使用し、拡張プロパティを含むリソース インスタンスを 1 つまたはコレクションで取得します](../api/singlevaluelegacyextendedproperty-get.md)

複数値の拡張プロパティの操作:

- [新規または既存のリソースのインスタンスに、拡張プロパティを作成します](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [`$expand` を使用して拡張プロパティを含むリソース インスタンスを取得します](../api/multivaluelegacyextendedproperty-get.md)

