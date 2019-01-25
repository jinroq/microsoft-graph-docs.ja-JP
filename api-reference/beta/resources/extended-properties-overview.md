---
title: Outlook の拡張プロパティの概要
description: '拡張プロパティは、カスタム データを格納できるようにして、アプリケーションにアクセスするためのフォールバック メカニズムとしてサービスの提供に '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ead40279547fa838b7224a25c3605d0825c3f797
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517996"
---
# <a name="outlook-extended-properties-overview"></a><span data-ttu-id="ba2f4-103">Outlook の拡張プロパティの概要</span><span class="sxs-lookup"><span data-stu-id="ba2f4-103">Outlook extended properties overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba2f4-p101">拡張プロパティではカスタム データを格納することができます。特に Outlook MAPI プロパティが_まだ Microsoft Graph API のメタデータで公開されていない_場合に、拡張プロパティは、アプリがこれらのプロパティのカスタム データにアクセスするためのフォールバック メカニズムとして機能します。拡張プロパティの REST API を使用して、次のユーザー リソースにこのようなカスタム データを格納したり、取得したりできます。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-p101">Extended properties allow storing custom data and specifically serve as a fallback mechanism for apps to access custom data for Outlook MAPI properties when these properties are _not already exposed in the Microsoft Graph API metadata_. You can use extended properties REST API to store or get such custom data in the following user resources:</span></span>

- [<span data-ttu-id="ba2f4-106">message</span><span class="sxs-lookup"><span data-stu-id="ba2f4-106">message</span></span>](../resources/message.md)
- [<span data-ttu-id="ba2f4-107">mailFolder</span><span class="sxs-lookup"><span data-stu-id="ba2f4-107">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="ba2f4-108">event</span><span class="sxs-lookup"><span data-stu-id="ba2f4-108">event</span></span>](../resources/event.md)
- [<span data-ttu-id="ba2f4-109">calendar</span><span class="sxs-lookup"><span data-stu-id="ba2f4-109">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="ba2f4-110">contact</span><span class="sxs-lookup"><span data-stu-id="ba2f4-110">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="ba2f4-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ba2f4-111">contactFolder</span></span>](../resources/contactfolder.md)
- <span data-ttu-id="ba2f4-112">Outlook タスク</span><span class="sxs-lookup"><span data-stu-id="ba2f4-112">[Outlook task](../resources/outlooktask.md)</span></span>
- [<span data-ttu-id="ba2f4-113">Outlook の仕事フォルダー</span><span class="sxs-lookup"><span data-stu-id="ba2f4-113">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) 

<span data-ttu-id="ba2f4-114">または、次の Office 365 グループ リソースとの間でもデータをやり取りできます。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-114">Or, in the following Office 365 group resources:</span></span>

- <span data-ttu-id="ba2f4-115">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="ba2f4-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="ba2f4-116">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="ba2f4-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="ba2f4-117">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="ba2f4-117">group [post](../resources/post.md)</span></span> 

## <a name="use-extended-properties-or-open-extensions"></a><span data-ttu-id="ba2f4-118">拡張プロパティとオープン拡張機能のどちらを使用するか</span><span class="sxs-lookup"><span data-stu-id="ba2f4-118">Use extended properties or open extensions?</span></span>

<span data-ttu-id="ba2f4-p102">最も一般的なシナリオとして、オープン拡張機能 ([openTypeExtension](../resources/opentypeextension.md) で表される。旧称は Office 365 のデータ拡張機能) を使用して、リソース インスタンスのカスタム データをユーザーのメールボックスに格納したり、それらにアクセスしたりできます。拡張プロパティは、[Microsoft Graph API のメタデータ](https://developer.microsoft.com/graph/docs/overview/call_api)でまだ公開されていない Outlook MAPI プロパティのカスタム データにアクセスする必要がある場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-p102">In most common scenarios, you should be able to use open extensions (represented by [openTypeExtension](../resources/opentypeextension.md), formerly known as Office 365 data extensions) to store and access custom data for resource instances in a user's mailbox. Use extended properties only if you need to access custom data for Outlook MAPI properties that are not already exposed in the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api).</span></span>

## <a name="types-of-extended-properties"></a><span data-ttu-id="ba2f4-121">拡張プロパティのタイプ</span><span class="sxs-lookup"><span data-stu-id="ba2f4-121">Types of extended properties</span></span>

<span data-ttu-id="ba2f4-122">拡張プロパティに単一の値を保存するか、または (同じ型の) 複数の値を保存するかに応じて、拡張プロパティを [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)、または [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) として作成できます。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-122">Depending on whether you intend to store a single or multiple values (of the same type) in an extended property, you can create an extended property as a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), or [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span></span>

<span data-ttu-id="ba2f4-123">これらのタイプはそれぞれ、**id** によってプロパティを識別し、データを **value** に格納します。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-123">Each of these types identifies the property by its **id** and stores data in **value**.</span></span> 

<span data-ttu-id="ba2f4-124">**id** を使用して、特定のリソース インスタンスをその拡張プロパティと一緒に取得するか、単一の値の拡張プロパティでフィルターして、そのプロパティのすべてのインスタンスを取得できます。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-124">You can use **id** to get a specific resource instance together with that extended property, or filter on a single-value extended property to get all the instances that have that property.</span></span> 

<span data-ttu-id="ba2f4-125">**注** REST API を使用して、1 つの呼び出しで特定のインスタンスのすべての拡張プロパティを取得することはできません。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-125">**Note** You cannot use the REST API to get all the extended properties of a specific instance in one call.</span></span>
  

### <a name="id-formats"></a><span data-ttu-id="ba2f4-126">id の形式</span><span class="sxs-lookup"><span data-stu-id="ba2f4-126">id formats</span></span>

<span data-ttu-id="ba2f4-127">3 つの形式のいずれかでは、拡張プロパティの**id**を指定できます。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-127">You can specify **id** of an extended property in one of three formats:</span></span>

- <span data-ttu-id="ba2f4-128">名前付きプロパティとして、拡張プロパティの型、名前空間、および文字列名によって識別します。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-128">As a named property, identified by the extended property type, namespace, and a string name.</span></span>
- <span data-ttu-id="ba2f4-129">名前付きプロパティとして、拡張プロパティの型、名前空間、および数値識別子によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-129">As a named property, identified by the extended property type, namespace, and a numeric identifier.</span></span>
- <span data-ttu-id="ba2f4-130">Proptag の形式で、拡張プロパティの型、および[MAPI プロパティ タグ](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags)で識別されます。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-130">In a proptag format, identified by the extended property type and a [MAPI property tag](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags).</span></span>

<span data-ttu-id="ba2f4-131">次の 2 つのテーブルは、単一および複数の値に適用されている拡張プロパティとして、これらの形式を記述します。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-131">The next 2 tables describe these formats as applied to single and multi-value extended properties.</span></span> <span data-ttu-id="ba2f4-132">{_タイプ_} では、拡張プロパティの値の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-132">{_type_} represents the type of the value or values of the extended property.</span></span> <span data-ttu-id="ba2f4-133">この例では、文字列、整数、およびこれらの種類の配列を示しています。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-133">Shown in the examples are string, integer, and arrays of these types.</span></span>

<span data-ttu-id="ba2f4-134">**単一値の拡張プロパティに有効な id の形式**</span><span class="sxs-lookup"><span data-stu-id="ba2f4-134">**Valid id formats for single-value extended properties**</span></span>

|<span data-ttu-id="ba2f4-135">**形式**</span><span class="sxs-lookup"><span data-stu-id="ba2f4-135">**Format**</span></span>|<span data-ttu-id="ba2f4-136">**例**</span><span class="sxs-lookup"><span data-stu-id="ba2f4-136">**Example**</span></span>|<span data-ttu-id="ba2f4-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="ba2f4-137">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="ba2f4-138">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="ba2f4-138">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="ba2f4-139">それが属している名前空間 (GUID) と文字列名によってプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-139">Identifies a property by the namespace (the GUID) it belongs to, and a string name.</span></span>         |
| <span data-ttu-id="ba2f4-140">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="ba2f4-140">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | <span data-ttu-id="ba2f4-141">プロパティが属している名前空間 (GUID) と数値の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-141">Identifies a property by the namespace (the GUID) it belongs to, and a numeric identifier.</span></span>  |
| <span data-ttu-id="ba2f4-142">[{_タイプ_} {_proptag_}]</span><span class="sxs-lookup"><span data-stu-id="ba2f4-142">"{_type_} {_proptag_}"</span></span>                    | ```"String 0x4001001E"```                                           | <span data-ttu-id="ba2f4-143">プロパティ タグを事前に定義されたプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-143">Identifies a pre-defined property by its property tag.</span></span> |

<span data-ttu-id="ba2f4-144">**複数値の拡張プロパティに有効な id の形式**</span><span class="sxs-lookup"><span data-stu-id="ba2f4-144">**Valid id formats for multi-value extended properties**</span></span>

|<span data-ttu-id="ba2f4-145">**形式**</span><span class="sxs-lookup"><span data-stu-id="ba2f4-145">**Format**</span></span>|<span data-ttu-id="ba2f4-146">**例**</span><span class="sxs-lookup"><span data-stu-id="ba2f4-146">**Example**</span></span>|<span data-ttu-id="ba2f4-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="ba2f4-147">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="ba2f4-148">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="ba2f4-148">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="ba2f4-149">名前空間 (GUID) と文字列名によってプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-149">Identifies a property by the namespace (the GUID) and a string name.</span></span>         |
| <span data-ttu-id="ba2f4-150">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="ba2f4-150">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | <span data-ttu-id="ba2f4-151">数値識別子 (GUID) の名前空間によってプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-151">Identifies a property by the namespace (the GUID) and a numeric identifier.</span></span>   |
| <span data-ttu-id="ba2f4-152">[{_タイプ_} {_proptag_}]</span><span class="sxs-lookup"><span data-stu-id="ba2f4-152">"{_type_} {_proptag_}"</span></span>                    | ```"StringArray 0x4002101E"```                                           | <span data-ttu-id="ba2f4-153">プロパティ タグを事前に定義されたプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-153">Identifies a pre-defined property by its property tag.</span></span> |


<span data-ttu-id="ba2f4-154">単一値または複数値の拡張プロパティをカスタム プロパティとして定義するのにには、名前付きプロパティの形式のいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-154">Use either of the named property formats to define a single-value or multi-value extended property as a custom property.</span></span> <span data-ttu-id="ba2f4-155">2 つの形式では、文字列の名前 (**名**) は、1 つ目は参照の容易にするために優先されるフォーマットがあります。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-155">Among the two formats, the first one that takes a string name (**Name**) is the preferred format for ease of reference.</span></span> <span data-ttu-id="ba2f4-156">名前付きプロパティでは、その[プロパティの識別子](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview)を持つ 0x8000-0 xfffe の範囲です。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-156">Named properties have their [property identifiers](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview) in the 0x8000-0xfffe range.</span></span>

<span data-ttu-id="ba2f4-157">Proptag 形式を使用して、MAPI、または、クライアントまたはサーバーで定義済みのプロパティにアクセスしてするが既に公開されていない Microsoft Graph で。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-157">Use the proptag format to access properties predefined by MAPI, or by a client or server, and that have not already been exposed in Microsoft Graph.</span></span> <span data-ttu-id="ba2f4-158">これらのプロパティでは、プロパティの識別子を持つ、0x0001 0x7fff の範囲です。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-158">These properties have property identifiers in the 0x0001-0x7fff range.</span></span> <span data-ttu-id="ba2f4-159">Proptag 形式を使用してカスタム プロパティを定義しないでください。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-159">Do not try to define a custom property using the proptag format.</span></span> 

<span data-ttu-id="ba2f4-160">
  \[MS-OXPROPS\] Microsoft Corporation の[「Exchange Server プロトコルのマスター プロパティ リスト」](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx)では、既存の MAPI プロパティへの拡張プロパティのマッピングに関する情報 (プロパティ識別子や GUID など) を検索できます。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-160">You can find information about mapping an extended property to an existing MAPI property, such as the property identifier and GUID, in \[MS-OXPROPS\] Microsoft Corporation, ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span></span>

<span data-ttu-id="ba2f4-161">**注** **id** に対して 1 つの形式を選択したら、その形式でのみ拡張プロパティにアクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="ba2f4-161">**Note** After you have chosen one format for the **id**, you should access that extended property by only that format.</span></span>

## <a name="rest-api-operations"></a><span data-ttu-id="ba2f4-162">REST API の操作</span><span class="sxs-lookup"><span data-stu-id="ba2f4-162">REST API operations</span></span>
 
<span data-ttu-id="ba2f4-163">単一値の拡張プロパティの操作:</span><span class="sxs-lookup"><span data-stu-id="ba2f4-163">Single-value extended property operations:</span></span>

- [<span data-ttu-id="ba2f4-164">新規または既存のリソースのインスタンスに、拡張プロパティを作成します</span><span class="sxs-lookup"><span data-stu-id="ba2f4-164">Create an extended property in a new or existing resource instance</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [<span data-ttu-id="ba2f4-165">`$expand` または `$filter` を使用し、拡張プロパティを含むリソース インスタンスを 1 つまたはコレクションで取得します</span><span class="sxs-lookup"><span data-stu-id="ba2f4-165">Get one or a collection of resource instances with an extended property using `$expand` or `$filter`</span></span>](../api/singlevaluelegacyextendedproperty-get.md)

<span data-ttu-id="ba2f4-166">複数値の拡張プロパティの操作:</span><span class="sxs-lookup"><span data-stu-id="ba2f4-166">Multi-value extended property operations:</span></span>

- [<span data-ttu-id="ba2f4-167">新規または既存のリソースのインスタンスに、拡張プロパティを作成します</span><span class="sxs-lookup"><span data-stu-id="ba2f4-167">Create an extended property in a new or existing resource instance</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [<span data-ttu-id="ba2f4-168">`$expand` を使用して拡張プロパティを含むリソース インスタンスを取得します</span><span class="sxs-lookup"><span data-stu-id="ba2f4-168">Get a resource instance with an extended property using `$expand`</span></span>](../api/multivaluelegacyextendedproperty-get.md)

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/extended-properties-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
