---
title: Outlook の拡張プロパティの概要
description: '拡張プロパティはカスタム データの保存を可能にし、特にアプリがアクセスできるようにフォールバック メカニズムとして機能します。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: eff117ac9b66121a7f0f383dd79dd6fe2a4270a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973598"
---
# <a name="outlook-extended-properties-overview"></a><span data-ttu-id="2f35e-103">Outlook の拡張プロパティの概要</span><span class="sxs-lookup"><span data-stu-id="2f35e-103">Outlook extended properties overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f35e-p101">拡張プロパティではカスタム データを格納することができます。特に Outlook MAPI プロパティが_まだ Microsoft Graph API のメタデータで公開されていない_場合に、拡張プロパティは、アプリがこれらのプロパティのカスタム データにアクセスするためのフォールバック メカニズムとして機能します。拡張プロパティの REST API を使用して、次のユーザー リソースにこのようなカスタム データを格納したり、取得したりできます。</span><span class="sxs-lookup"><span data-stu-id="2f35e-p101">Extended properties allow storing custom data and specifically serve as a fallback mechanism for apps to access custom data for Outlook MAPI properties when these properties are _not already exposed in the Microsoft Graph API metadata_. You can use extended properties REST API to store or get such custom data in the following user resources:</span></span>

- [<span data-ttu-id="2f35e-106">message</span><span class="sxs-lookup"><span data-stu-id="2f35e-106">message</span></span>](../resources/message.md)
- [<span data-ttu-id="2f35e-107">mailFolder</span><span class="sxs-lookup"><span data-stu-id="2f35e-107">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="2f35e-108">event</span><span class="sxs-lookup"><span data-stu-id="2f35e-108">event</span></span>](../resources/event.md)
- [<span data-ttu-id="2f35e-109">calendar</span><span class="sxs-lookup"><span data-stu-id="2f35e-109">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="2f35e-110">contact</span><span class="sxs-lookup"><span data-stu-id="2f35e-110">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="2f35e-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="2f35e-111">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="2f35e-112">Outlook タスク</span><span class="sxs-lookup"><span data-stu-id="2f35e-112">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="2f35e-113">Outlook タスク フォルダー</span><span class="sxs-lookup"><span data-stu-id="2f35e-113">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) 

<span data-ttu-id="2f35e-114">または、次の Office 365 グループ リソースとの間でもデータをやり取りできます。</span><span class="sxs-lookup"><span data-stu-id="2f35e-114">Or, in the following Office 365 group resources:</span></span>

- <span data-ttu-id="2f35e-115">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="2f35e-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="2f35e-116">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="2f35e-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="2f35e-117">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="2f35e-117">group [post](../resources/post.md)</span></span> 

## <a name="use-extended-properties-or-open-extensions"></a><span data-ttu-id="2f35e-118">拡張プロパティとオープン拡張機能のどちらを使用するか</span><span class="sxs-lookup"><span data-stu-id="2f35e-118">Use extended properties or open extensions?</span></span>

<span data-ttu-id="2f35e-p102">最も一般的なシナリオとして、オープン拡張機能 ([openTypeExtension](../resources/opentypeextension.md) で表される。旧称は Office 365 のデータ拡張機能) を使用して、リソース インスタンスのカスタム データをユーザーのメールボックスに格納したり、それらにアクセスしたりできます。拡張プロパティは、[Microsoft Graph API のメタデータ](https://developer.microsoft.com/graph/docs/overview/call_api)でまだ公開されていない Outlook MAPI プロパティのカスタム データにアクセスする必要がある場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="2f35e-p102">In most common scenarios, you should be able to use open extensions (represented by [openTypeExtension](../resources/opentypeextension.md), formerly known as Office 365 data extensions) to store and access custom data for resource instances in a user's mailbox. Use extended properties only if you need to access custom data for Outlook MAPI properties that are not already exposed in the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api).</span></span>

## <a name="types-of-extended-properties"></a><span data-ttu-id="2f35e-121">拡張プロパティのタイプ</span><span class="sxs-lookup"><span data-stu-id="2f35e-121">Types of extended properties</span></span>

<span data-ttu-id="2f35e-122">拡張プロパティに単一の値を保存するか、または (同じ型の) 複数の値を保存するかに応じて、拡張プロパティを [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)、または [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) として作成できます。</span><span class="sxs-lookup"><span data-stu-id="2f35e-122">Depending on whether you intend to store a single or multiple values (of the same type) in an extended property, you can create an extended property as a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), or [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span></span>

<span data-ttu-id="2f35e-123">これらのタイプはそれぞれ、**id** によってプロパティを識別し、データを **value** に格納します。</span><span class="sxs-lookup"><span data-stu-id="2f35e-123">Each of these types identifies the property by its **id** and stores data in **value**.</span></span> 

<span data-ttu-id="2f35e-124">**id** を使用して、特定のリソース インスタンスをその拡張プロパティと一緒に取得するか、単一の値の拡張プロパティでフィルターして、そのプロパティのすべてのインスタンスを取得できます。</span><span class="sxs-lookup"><span data-stu-id="2f35e-124">You can use **id** to get a specific resource instance together with that extended property, or filter on a single-value extended property to get all the instances that have that property.</span></span> 

<span data-ttu-id="2f35e-125">**注** REST API を使用して、1 つの呼び出しで特定のインスタンスのすべての拡張プロパティを取得することはできません。</span><span class="sxs-lookup"><span data-stu-id="2f35e-125">**Note** You cannot use the REST API to get all the extended properties of a specific instance in one call.</span></span>
  

### <a name="id-formats"></a><span data-ttu-id="2f35e-126">id の形式</span><span class="sxs-lookup"><span data-stu-id="2f35e-126">id formats</span></span>

<span data-ttu-id="2f35e-127">拡張プロパティの **id** は、次の 3 つの形式のいずれかで指定することができます。</span><span class="sxs-lookup"><span data-stu-id="2f35e-127">You can specify **id** of an extended property in one of three formats:</span></span>

- <span data-ttu-id="2f35e-128">名前付きプロパティ - 拡張プロパティの種類、名前空間、および文字列名によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="2f35e-128">As a named property, identified by the extended property type, namespace, and a string name.</span></span>
- <span data-ttu-id="2f35e-129">名前付きプロパティ - 拡張プロパティの種類、名前空間、および数値の識別子によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="2f35e-129">As a named property, identified by the extended property type, namespace, and a numeric identifier.</span></span>
- <span data-ttu-id="2f35e-130">proptag の形式 - 拡張プロパティの種類、および [MAPI プロパティのタグ](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags)によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="2f35e-130">In a proptag format, identified by the extended property type and a [MAPI property tag](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags).</span></span>

<span data-ttu-id="2f35e-131">次の 2 つの表では、単一値または複数値の拡張プロパティに適用されるこれらの形式について説明します。</span><span class="sxs-lookup"><span data-stu-id="2f35e-131">The next 2 tables describe these formats as applied to single and multi-value extended properties.</span></span> <span data-ttu-id="2f35e-132">{_type_} は、拡張プロパティ値の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="2f35e-132">{_type_} represents the type of the value or values of the extended property.</span></span> <span data-ttu-id="2f35e-133">この例では、これらの種類の文字列、整数、および配列を示しています。</span><span class="sxs-lookup"><span data-stu-id="2f35e-133">Shown in the examples are string, integer, and arrays of these types.</span></span>

<span data-ttu-id="2f35e-134">**単一値の拡張プロパティに有効な id の形式**</span><span class="sxs-lookup"><span data-stu-id="2f35e-134">**Valid id formats for single-value extended properties**</span></span>

|<span data-ttu-id="2f35e-135">**形式**</span><span class="sxs-lookup"><span data-stu-id="2f35e-135">**Format**</span></span>|<span data-ttu-id="2f35e-136">**例**</span><span class="sxs-lookup"><span data-stu-id="2f35e-136">**Example**</span></span>|<span data-ttu-id="2f35e-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="2f35e-137">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="2f35e-138">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="2f35e-138">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="2f35e-139">属している名前空間 (GUID) と文字列の名前で、プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="2f35e-139">Identifies a property by the namespace (the GUID) it belongs to, and a string name.</span></span>         |
| <span data-ttu-id="2f35e-140">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="2f35e-140">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | <span data-ttu-id="2f35e-141">属している名前空間 (GUID) と数値の識別子で、プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="2f35e-141">Identifies a property by the namespace (the GUID) it belongs to, and a numeric identifier.</span></span>  |
| <span data-ttu-id="2f35e-142">"{_type_} {_proptag_}"</span><span class="sxs-lookup"><span data-stu-id="2f35e-142">"{_type_} {_proptag_}"</span></span>                    | ```"String 0x4001001E"```                                           | <span data-ttu-id="2f35e-143">事前定義済みプロパティをそのプロパティ タグで識別します。</span><span class="sxs-lookup"><span data-stu-id="2f35e-143">Identifies a pre-defined property by its property tag.</span></span> |

<span data-ttu-id="2f35e-144">**複数値の拡張プロパティに有効な id の形式**</span><span class="sxs-lookup"><span data-stu-id="2f35e-144">**Valid id formats for multi-value extended properties**</span></span>

|<span data-ttu-id="2f35e-145">**形式**</span><span class="sxs-lookup"><span data-stu-id="2f35e-145">**Format**</span></span>|<span data-ttu-id="2f35e-146">**例**</span><span class="sxs-lookup"><span data-stu-id="2f35e-146">**Example**</span></span>|<span data-ttu-id="2f35e-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="2f35e-147">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="2f35e-148">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="2f35e-148">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="2f35e-149">名前空間 (GUID) と文字列の名前で、プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="2f35e-149">Identifies a property by the namespace (the GUID) and a string name.</span></span>         |
| <span data-ttu-id="2f35e-150">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="2f35e-150">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | <span data-ttu-id="2f35e-151">名前空間 (GUID) と数値の識別子で、プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="2f35e-151">Identifies a property by the namespace (the GUID) and a numeric identifier.</span></span>   |
| <span data-ttu-id="2f35e-152">"{_type_} {_proptag_}"</span><span class="sxs-lookup"><span data-stu-id="2f35e-152">"{_type_} {_proptag_}"</span></span>                    | ```"StringArray 0x4002101E"```                                           | <span data-ttu-id="2f35e-153">事前定義済みプロパティをそのプロパティ タグで識別します。</span><span class="sxs-lookup"><span data-stu-id="2f35e-153">Identifies a pre-defined property by its property tag.</span></span> |


<span data-ttu-id="2f35e-154">名前付きプロパティ形式のいずれかを使用して、単一値または複数値の拡張プロパティをカスタム プロパティとして定義します。</span><span class="sxs-lookup"><span data-stu-id="2f35e-154">Use either of the named property formats to define a single-value or multi-value extended property as a custom property.</span></span> <span data-ttu-id="2f35e-155">2 つの形式のうち、文字列名 (**Name**) を先にとる形式の方が参照しやすいため、推奨形式となります。</span><span class="sxs-lookup"><span data-stu-id="2f35e-155">Among the two formats, the first one that takes a string name (**Name**) is the preferred format for ease of reference.</span></span> <span data-ttu-id="2f35e-156">名前付きプロパティの[プロパティの識別子](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview)は、0x8000-0xfffe の範囲にあります。</span><span class="sxs-lookup"><span data-stu-id="2f35e-156">Named properties have their [property identifiers](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview) in the 0x8000-0xfffe range.</span></span>

<span data-ttu-id="2f35e-157">MAPI によって、またはクライアントまたはサーバーによって事前定義済みの、まだ Microsoft Graph に公開されていないプロパティにアクセスするには、proptag 形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="2f35e-157">Use the proptag format to access properties predefined by MAPI, or by a client or server, and that have not already been exposed in Microsoft Graph.</span></span> <span data-ttu-id="2f35e-158">これらのプロパティのプロパティ識別子は、0x0001〜0x7fff の範囲にあります。</span><span class="sxs-lookup"><span data-stu-id="2f35e-158">These properties have property identifiers in the 0x0001-0x7fff range.</span></span> <span data-ttu-id="2f35e-159">カスタム プロパティを定義するのに、proptag 形式を使用してしないでください。</span><span class="sxs-lookup"><span data-stu-id="2f35e-159">Do not try to define a custom property using the proptag format.</span></span> 

<span data-ttu-id="2f35e-160">\[MS-OXPROPS\] Microsoft Corporation の[「Exchange Server プロトコルのマスター プロパティ リスト」](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx)では、既存の MAPI プロパティへの拡張プロパティのマッピングに関する情報 (プロパティ識別子や GUID など) を検索できます。</span><span class="sxs-lookup"><span data-stu-id="2f35e-160">You can find information about mapping an extended property to an existing MAPI property, such as the property identifier and GUID, in \[MS-OXPROPS\] Microsoft Corporation, ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span></span>

<span data-ttu-id="2f35e-161">**注** **id** に対して 1 つの形式を選択したら、その形式でのみ拡張プロパティにアクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="2f35e-161">**Note** After you have chosen one format for the **id**, you should access that extended property by only that format.</span></span>

## <a name="rest-api-operations"></a><span data-ttu-id="2f35e-162">REST API の操作</span><span class="sxs-lookup"><span data-stu-id="2f35e-162">REST API operations</span></span>
 
<span data-ttu-id="2f35e-163">単一値の拡張プロパティの操作:</span><span class="sxs-lookup"><span data-stu-id="2f35e-163">Single-value extended property operations:</span></span>

- [<span data-ttu-id="2f35e-164">新規または既存のリソースのインスタンスに、拡張プロパティを作成します</span><span class="sxs-lookup"><span data-stu-id="2f35e-164">Create an extended property in a new or existing resource instance</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [<span data-ttu-id="2f35e-165">`$expand` または `$filter` を使用し、拡張プロパティを含むリソース インスタンスを 1 つまたはコレクションで取得します</span><span class="sxs-lookup"><span data-stu-id="2f35e-165">Get one or a collection of resource instances with an extended property using `$expand` or `$filter`</span></span>](../api/singlevaluelegacyextendedproperty-get.md)

<span data-ttu-id="2f35e-166">複数値の拡張プロパティの操作:</span><span class="sxs-lookup"><span data-stu-id="2f35e-166">Multi-value extended property operations:</span></span>

- [<span data-ttu-id="2f35e-167">新規または既存のリソースのインスタンスに、拡張プロパティを作成します</span><span class="sxs-lookup"><span data-stu-id="2f35e-167">Create an extended property in a new or existing resource instance</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [<span data-ttu-id="2f35e-168">`$expand` を使用して拡張プロパティを含むリソース インスタンスを取得します</span><span class="sxs-lookup"><span data-stu-id="2f35e-168">Get a resource instance with an extended property using `$expand`</span></span>](../api/multivaluelegacyextendedproperty-get.md)

