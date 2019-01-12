---
title: Outlook の拡張プロパティの概要
description: '拡張プロパティは、カスタム データを格納できるようにして、アプリケーションにアクセスするためのフォールバック メカニズムとしてサービスの提供に '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 935f97819155318a6bfc7c77d07bf8a308e512e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949571"
---
# <a name="outlook-extended-properties-overview"></a><span data-ttu-id="427f7-103">Outlook の拡張プロパティの概要</span><span class="sxs-lookup"><span data-stu-id="427f7-103">Outlook extended properties overview</span></span>

<span data-ttu-id="427f7-p101">拡張プロパティではカスタム データを格納することができます。特に Outlook MAPI プロパティが_まだ Microsoft Graph API のメタデータで公開されていない_場合に、拡張プロパティは、アプリがこれらのプロパティのカスタム データにアクセスするためのフォールバック メカニズムとして機能します。拡張プロパティの REST API を使用して、次のユーザー リソースにこのようなカスタム データを格納したり、取得したりできます。</span><span class="sxs-lookup"><span data-stu-id="427f7-p101">Extended properties allow storing custom data and specifically serve as a fallback mechanism for apps to access custom data for Outlook MAPI properties when these properties are _not already exposed in the Microsoft Graph API metadata_. You can use extended properties REST API to store or get such custom data in the following user resources:</span></span>

- [<span data-ttu-id="427f7-106">message</span><span class="sxs-lookup"><span data-stu-id="427f7-106">message</span></span>](../resources/message.md)
- [<span data-ttu-id="427f7-107">mailFolder</span><span class="sxs-lookup"><span data-stu-id="427f7-107">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="427f7-108">event</span><span class="sxs-lookup"><span data-stu-id="427f7-108">event</span></span>](../resources/event.md)
- [<span data-ttu-id="427f7-109">calendar</span><span class="sxs-lookup"><span data-stu-id="427f7-109">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="427f7-110">contact</span><span class="sxs-lookup"><span data-stu-id="427f7-110">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="427f7-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="427f7-111">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="427f7-112">または、次の Office 365 グループ リソースとの間でもデータをやり取りできます。</span><span class="sxs-lookup"><span data-stu-id="427f7-112">Or, in the following Office 365 group resources:</span></span>

- <span data-ttu-id="427f7-113">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="427f7-113">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="427f7-114">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="427f7-114">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="427f7-115">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="427f7-115">group [post](../resources/post.md)</span></span> 

## <a name="use-extended-properties-or-open-extensions"></a><span data-ttu-id="427f7-116">拡張プロパティとオープン拡張機能のどちらを使用するか</span><span class="sxs-lookup"><span data-stu-id="427f7-116">Use extended properties or open extensions?</span></span>

<span data-ttu-id="427f7-p102">最も一般的なシナリオとして、オープン拡張機能 ([openTypeExtension](../resources/opentypeextension.md) で表される。旧称は Office 365 のデータ拡張機能) を使用して、リソース インスタンスのカスタム データをユーザーのメールボックスに格納したり、それらにアクセスしたりできます。拡張プロパティは、[Microsoft Graph API のメタデータ](https://developer.microsoft.com/graph/docs/overview/call_api)でまだ公開されていない Outlook MAPI プロパティのカスタム データにアクセスする必要がある場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="427f7-p102">In most common scenarios, you should be able to use open extensions (represented by [openTypeExtension](../resources/opentypeextension.md), formerly known as Office 365 data extensions) to store and access custom data for resource instances in a user's mailbox. Use extended properties only if you need to access custom data for Outlook MAPI properties that are not already exposed in the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api).</span></span> 

## <a name="types-of-extended-properties"></a><span data-ttu-id="427f7-119">拡張プロパティのタイプ</span><span class="sxs-lookup"><span data-stu-id="427f7-119">Types of extended properties</span></span>

<span data-ttu-id="427f7-120">拡張プロパティに単一の値を保存するか、または (同じ型の) 複数の値を保存するかに応じて、拡張プロパティを [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)、または [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) として作成できます。</span><span class="sxs-lookup"><span data-stu-id="427f7-120">Depending on whether you intend to store a single or multiple values (of the same type) in an extended property, you can create an extended property as a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), or [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span></span>

<span data-ttu-id="427f7-121">これらのタイプはそれぞれ、**id** によってプロパティを識別し、データを **value** に格納します。</span><span class="sxs-lookup"><span data-stu-id="427f7-121">Each of these types identifies the property by its **id** and stores data in **value**.</span></span> 

<span data-ttu-id="427f7-122">**id** を使用して、特定のリソース インスタンスをその拡張プロパティと一緒に取得するか、単一の値の拡張プロパティでフィルターして、そのプロパティのすべてのインスタンスを取得できます。</span><span class="sxs-lookup"><span data-stu-id="427f7-122">You can use **id** to get a specific resource instance together with that extended property, or filter on a single-value extended property to get all the instances that have that property.</span></span> 

<span data-ttu-id="427f7-123">**注** REST API を使用して、1 つの呼び出しで特定のインスタンスのすべての拡張プロパティを取得することはできません。</span><span class="sxs-lookup"><span data-stu-id="427f7-123">**Note** You cannot use the REST API to get all the extended properties of a specific instance in one call.</span></span>
  

### <a name="id-formats"></a><span data-ttu-id="427f7-124">id の形式</span><span class="sxs-lookup"><span data-stu-id="427f7-124">id formats</span></span>

<span data-ttu-id="427f7-125">3 つの形式のいずれかでは、拡張プロパティの**id**を指定できます。</span><span class="sxs-lookup"><span data-stu-id="427f7-125">You can specify **id** of an extended property in one of three formats:</span></span>

- <span data-ttu-id="427f7-126">名前付きプロパティとして、拡張プロパティの型、名前空間、および文字列名によって識別します。</span><span class="sxs-lookup"><span data-stu-id="427f7-126">As a named property, identified by the extended property type, namespace, and a string name.</span></span>
- <span data-ttu-id="427f7-127">名前付きプロパティとして、拡張プロパティの型、名前空間、および数値識別子によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="427f7-127">As a named property, identified by the extended property type, namespace, and a numeric identifier.</span></span>
- <span data-ttu-id="427f7-128">Proptag の形式で、拡張プロパティの型、および[MAPI プロパティ タグ](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags)で識別されます。</span><span class="sxs-lookup"><span data-stu-id="427f7-128">In a proptag format, identified by the extended property type and a [MAPI property tag](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags).</span></span>

<span data-ttu-id="427f7-129">次の 2 つのテーブルは、単一および複数の値に適用されている拡張プロパティとして、これらの形式を記述します。</span><span class="sxs-lookup"><span data-stu-id="427f7-129">The next 2 tables describe these formats as applied to single and multi-value extended properties.</span></span> <span data-ttu-id="427f7-130">{_タイプ_} では、拡張プロパティの値の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="427f7-130">{_type_} represents the type of the value or values of the extended property.</span></span> <span data-ttu-id="427f7-131">この例では、文字列、整数、およびこれらの種類の配列を示しています。</span><span class="sxs-lookup"><span data-stu-id="427f7-131">Shown in the examples are string, integer, and arrays of these types.</span></span>

<span data-ttu-id="427f7-132">**単一値の拡張プロパティに有効な id の形式**</span><span class="sxs-lookup"><span data-stu-id="427f7-132">**Valid id formats for single-value extended properties**</span></span>

|<span data-ttu-id="427f7-133">**形式**</span><span class="sxs-lookup"><span data-stu-id="427f7-133">**Format**</span></span>|<span data-ttu-id="427f7-134">**例**</span><span class="sxs-lookup"><span data-stu-id="427f7-134">**Example**</span></span>|<span data-ttu-id="427f7-135">**説明**</span><span class="sxs-lookup"><span data-stu-id="427f7-135">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="427f7-136">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="427f7-136">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="427f7-137">それが属している名前空間 (GUID) と文字列名によってプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="427f7-137">Identifies a property by the namespace (the GUID) it belongs to, and a string name.</span></span>         |
| <span data-ttu-id="427f7-138">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="427f7-138">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | <span data-ttu-id="427f7-139">プロパティが属している名前空間 (GUID) と数値の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="427f7-139">Identifies a property by the namespace (the GUID) it belongs to, and a numeric identifier.</span></span>  |
| <span data-ttu-id="427f7-140">[{_タイプ_} {_proptag_}]</span><span class="sxs-lookup"><span data-stu-id="427f7-140">"{_type_} {_proptag_}"</span></span>                    | ```"String 0x4001001E"```                                           | <span data-ttu-id="427f7-141">プロパティ タグを事前に定義されたプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="427f7-141">Identifies a pre-defined property by its property tag.</span></span> |

<span data-ttu-id="427f7-142">**複数値の拡張プロパティに有効な id の形式**</span><span class="sxs-lookup"><span data-stu-id="427f7-142">**Valid id formats for multi-value extended properties**</span></span>

|<span data-ttu-id="427f7-143">**形式**</span><span class="sxs-lookup"><span data-stu-id="427f7-143">**Format**</span></span>|<span data-ttu-id="427f7-144">**例**</span><span class="sxs-lookup"><span data-stu-id="427f7-144">**Example**</span></span>|<span data-ttu-id="427f7-145">**説明**</span><span class="sxs-lookup"><span data-stu-id="427f7-145">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="427f7-146">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="427f7-146">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="427f7-147">名前空間 (GUID) と文字列名によってプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="427f7-147">Identifies a property by the namespace (the GUID) and a string name.</span></span>         |
| <span data-ttu-id="427f7-148">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="427f7-148">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | <span data-ttu-id="427f7-149">数値識別子 (GUID) の名前空間によってプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="427f7-149">Identifies a property by the namespace (the GUID) and a numeric identifier.</span></span>   |
| <span data-ttu-id="427f7-150">[{_タイプ_} {_proptag_}]</span><span class="sxs-lookup"><span data-stu-id="427f7-150">"{_type_} {_proptag_}"</span></span>                    | ```"StringArray 0x4002101E"```                                           | <span data-ttu-id="427f7-151">プロパティ タグを事前に定義されたプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="427f7-151">Identifies a pre-defined property by its property tag.</span></span> |


<span data-ttu-id="427f7-152">単一値または複数値の拡張プロパティをカスタム プロパティとして定義するのにには、名前付きプロパティの形式のいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="427f7-152">Use either of the named property formats to define a single-value or multi-value extended property as a custom property.</span></span> <span data-ttu-id="427f7-153">2 つの形式では、文字列の名前 (**名**) は、1 つ目は参照の容易にするために優先されるフォーマットがあります。</span><span class="sxs-lookup"><span data-stu-id="427f7-153">Among the two formats, the first one that takes a string name (**Name**) is the preferred format for ease of reference.</span></span> <span data-ttu-id="427f7-154">名前付きプロパティでは、その[プロパティの識別子](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview)を持つ 0x8000-0 xfffe の範囲です。</span><span class="sxs-lookup"><span data-stu-id="427f7-154">Named properties have their [property identifiers](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview) in the 0x8000-0xfffe range.</span></span>

<span data-ttu-id="427f7-155">Proptag 形式を使用して、MAPI、または、クライアントまたはサーバーで定義済みのプロパティにアクセスしてするが既に公開されていない Microsoft Graph で。</span><span class="sxs-lookup"><span data-stu-id="427f7-155">Use the proptag format to access properties predefined by MAPI, or by a client or server, and that have not already been exposed in Microsoft Graph.</span></span> <span data-ttu-id="427f7-156">これらのプロパティでは、プロパティの識別子を持つ、0x0001 0x7fff の範囲です。</span><span class="sxs-lookup"><span data-stu-id="427f7-156">These properties have property identifiers in the 0x0001-0x7fff range.</span></span> <span data-ttu-id="427f7-157">Proptag 形式を使用してカスタム プロパティを定義しないでください。</span><span class="sxs-lookup"><span data-stu-id="427f7-157">Do not try to define a custom property using the proptag format.</span></span> 

<span data-ttu-id="427f7-158">
  \[MS-OXPROPS\] Microsoft Corporation の[「Exchange Server プロトコルのマスター プロパティ リスト」](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx)では、既存の MAPI プロパティへの拡張プロパティのマッピングに関する情報 (プロパティ識別子や GUID など) を検索できます。</span><span class="sxs-lookup"><span data-stu-id="427f7-158">You can find information about mapping an extended property to an existing MAPI property, such as the property identifier and GUID, in \[MS-OXPROPS\] Microsoft Corporation, ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span></span>

<span data-ttu-id="427f7-159">**注** **id** に対して 1 つの形式を選択したら、その形式でのみ拡張プロパティにアクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="427f7-159">**Note** After you have chosen one format for the **id**, you should access that extended property by only that format.</span></span>

### <a name="rest-api-operations"></a><span data-ttu-id="427f7-160">REST API の操作</span><span class="sxs-lookup"><span data-stu-id="427f7-160">REST API operations</span></span>
 
<span data-ttu-id="427f7-161">単一値の拡張プロパティの操作:</span><span class="sxs-lookup"><span data-stu-id="427f7-161">Single-value extended property operations:</span></span>

- [<span data-ttu-id="427f7-162">新規または既存のリソースのインスタンスに、拡張プロパティを作成します</span><span class="sxs-lookup"><span data-stu-id="427f7-162">Create an extended property in a new or existing resource instance</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [<span data-ttu-id="427f7-163">`$expand` または `$filter` を使用し、拡張プロパティを含むリソース インスタンスを 1 つまたはコレクションで取得します</span><span class="sxs-lookup"><span data-stu-id="427f7-163">Get one or a collection of resource instances with an extended property using `$expand` or `$filter`</span></span>](../api/singlevaluelegacyextendedproperty-get.md)

<span data-ttu-id="427f7-164">複数値の拡張プロパティの操作:</span><span class="sxs-lookup"><span data-stu-id="427f7-164">Multi-value extended property operations:</span></span>

- [<span data-ttu-id="427f7-165">新規または既存のリソースのインスタンスに、拡張プロパティを作成します</span><span class="sxs-lookup"><span data-stu-id="427f7-165">Create an extended property in a new or existing resource instance</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [<span data-ttu-id="427f7-166">`$expand` を使用して拡張プロパティを含むリソース インスタンスを取得します</span><span class="sxs-lookup"><span data-stu-id="427f7-166">Get a resource instance with an extended property using `$expand`</span></span>](../api/multivaluelegacyextendedproperty-get.md)

