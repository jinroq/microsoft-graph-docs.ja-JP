---
title: Outlook の拡張プロパティの概要
description: '拡張プロパティを使用してカスタムデータを保存し、特にアプリがアクセスするためのフォールバックメカニズムとして機能する '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 38aefd484d4afe13418255aa1d6e0b46050ae4fe
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340326"
---
# <a name="outlook-extended-properties-overview"></a>Outlook の拡張プロパティの概要

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

拡張プロパティではカスタム データを格納することができます。特に Outlook MAPI プロパティが_まだ Microsoft Graph API のメタデータで公開されていない_場合に、拡張プロパティは、アプリがこれらのプロパティのカスタム データにアクセスするためのフォールバック メカニズムとして機能します。拡張プロパティの REST API を使用して、次のユーザー リソースにこのようなカスタム データを格納したり、取得したりできます。

- [message](../resources/message.md)
- [mailFolder](../resources/mailfolder.md)
- [event](../resources/event.md)
- [calendar](../resources/calendar.md)
- [contact](../resources/contact.md)
- [contactFolder](../resources/contactfolder.md)
- [Outlook タスク](../resources/outlooktask.md)
- [Outlook タスク フォルダー](../resources/outlooktaskfolder.md) 

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

拡張プロパティの**id**は、次の3つの形式のいずれかで指定できます。

- 名前付きプロパティとして、拡張プロパティの型、名前空間、および文字列名で識別されます。
- 名前付きプロパティとして、拡張プロパティの型、名前空間、および数値識別子で識別されます。
- proptag 形式 (拡張プロパティの種類と[MAPI プロパティタグ](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags)によって識別されます)。

次の2つの表では、単一および複数値の拡張プロパティに適用されるこれらの形式について説明します。 {_type_} は、拡張プロパティの値または値の種類を表します。 この例では、文字列、整数、およびこれらの種類の配列を示しています。

**単一値の拡張プロパティに有効な id の形式**

|**形式**|**使用例**|**説明**|
|:---------|:----------|:--------------|
| "{_type_} {_guid_} **Name** {_name_}" | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | が属している名前空間 (GUID) と文字列名によってプロパティを識別します。         |
| "{_type_} {_guid_} **Id** {_id_}"     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | 属している名前空間 (GUID) と数値識別子によってプロパティを識別します。  |
| "{_type_} {_proptag_}"                    | ```"String 0x4001001E"```                                           | プロパティタグによって定義済みのプロパティを識別します。 |

**複数値の拡張プロパティに有効な id の形式**

|**形式**|**使用例**|**説明**|
|:---------|:----------|:--------------|
| "{_type_} {_guid_} **Name** {_name_}" | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | 名前空間 (GUID) と文字列名によってプロパティを識別します。         |
| "{_type_} {_guid_} **Id** {_id_}"     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | 名前空間 (GUID) と数値識別子によってプロパティを識別します。   |
| "{_type_} {_proptag_}"                    | ```"StringArray 0x4002101E"```                                           | プロパティタグによって定義済みのプロパティを識別します。 |


単一値または複数値の拡張プロパティをカスタムプロパティとして定義するには、名前付きプロパティの形式のいずれかを使用します。 2つの形式のうち、最初に文字列名 (**名前**) を取得する方法は、参照しやすいように推奨される形式です。 名前付きプロパティの[プロパティ識別子](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview)は、0xfffe の範囲内にあります。

proptag 形式を使用して、MAPI またはクライアントまたはサーバーによって定義済みのプロパティにアクセスし、Microsoft Graph ではまだ公開されていません。 これらのプロパティには、0x0001 の範囲内のプロパティ識別子があります。 proptag 形式を使用してカスタムプロパティを定義しないようにしてください。 


  \[MS-OXPROPS\] Microsoft Corporation の[「Exchange Server プロトコルのマスター プロパティ リスト」](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx)では、既存の MAPI プロパティへの拡張プロパティのマッピングに関する情報 (プロパティ識別子や GUID など) を検索できます。

**注** **id** に対して 1 つの形式を選択したら、その形式でのみ拡張プロパティにアクセスする必要があります。

## <a name="rest-api-operations"></a>REST API の操作
 
単一値の拡張プロパティの操作:

- [新規または既存のリソースのインスタンスに、拡張プロパティを作成します](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [`$expand` または `$filter` を使用し、拡張プロパティを含むリソース インスタンスを 1 つまたはコレクションで取得します](../api/singlevaluelegacyextendedproperty-get.md)

複数値の拡張プロパティの操作:

- [新規または既存のリソースのインスタンスに、拡張プロパティを作成します](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [`$expand` を使用して拡張プロパティを含むリソース インスタンスを取得します](../api/multivaluelegacyextendedproperty-get.md)

