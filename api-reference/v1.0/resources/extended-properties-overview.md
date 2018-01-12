# <a name="outlook-extended-properties-overview"></a><span data-ttu-id="26e05-101">Outlook の拡張プロパティの概要</span><span class="sxs-lookup"><span data-stu-id="26e05-101">Outlook extended properties overview</span></span>

<span data-ttu-id="26e05-p101">拡張プロパティではカスタム データを格納することができます。特に Outlook MAPI プロパティが_まだ Microsoft Graph API のメタデータで公開されていない_場合に、拡張プロパティは、アプリがこれらのプロパティのカスタム データにアクセスするためのフォールバック メカニズムとして機能します。拡張プロパティの REST API を使用して、次のユーザー リソースにこのようなカスタム データを格納したり、取得したりできます。</span><span class="sxs-lookup"><span data-stu-id="26e05-p101">Extended properties allow storing custom data and specifically serve as a fallback mechanism for apps to access custom data for Outlook MAPI properties when these properties are _not already exposed in the Microsoft Graph API metadata_. You can use extended properties REST API to store or get such custom data in the following user resources:</span></span>

- [<span data-ttu-id="26e05-104">message</span><span class="sxs-lookup"><span data-stu-id="26e05-104">message</span></span>](../resources/message.md)
- [<span data-ttu-id="26e05-105">mailFolder</span><span class="sxs-lookup"><span data-stu-id="26e05-105">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="26e05-106">event</span><span class="sxs-lookup"><span data-stu-id="26e05-106">event</span></span>](../resources/event.md)
- [<span data-ttu-id="26e05-107">calendar</span><span class="sxs-lookup"><span data-stu-id="26e05-107">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="26e05-108">contact</span><span class="sxs-lookup"><span data-stu-id="26e05-108">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="26e05-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="26e05-109">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="26e05-110">または、次の Office 365 グループ リソースとの間でもデータをやり取りできます。</span><span class="sxs-lookup"><span data-stu-id="26e05-110">Or, in the following Office 365 group resources:</span></span>

- <span data-ttu-id="26e05-111">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="26e05-111">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="26e05-112">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="26e05-112">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="26e05-113">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="26e05-113">group [post](../resources/post.md)</span></span> 

## <a name="use-extended-properties-or-open-extensions"></a><span data-ttu-id="26e05-114">拡張プロパティとオープン拡張機能のどちらを使用するか</span><span class="sxs-lookup"><span data-stu-id="26e05-114">Use extended properties or open extensions?</span></span>

<span data-ttu-id="26e05-p102">最も一般的なシナリオとして、オープン拡張機能 ([openTypeExtension](../resources/opentypeextension.md) で表される。旧称は Office 365 のデータ拡張機能) を使用して、リソース インスタンスのカスタム データをユーザーのメールボックスに格納したり、それらにアクセスしたりできます。拡張プロパティは、[Microsoft Graph API のメタデータ]((http://developer.microsoft.com/ja-JP/graph/docs/overview/call_api))でまだ公開されていない Outlook MAPI プロパティのカスタム データにアクセスする必要がある場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="26e05-p102">In most common scenarios, you should be able to use open extensions (represented by [openTypeExtension](../resources/opentypeextension.md), formerly known as Office 365 data extensions) to store and access custom data for resource instances in a user's mailbox. Use extended properties only if you need to access custom data for Outlook MAPI properties that are not already exposed in the [Microsoft Graph API metadata]((http://developer.microsoft.com/ja-JP/graph/docs/overview/call_api)).</span></span> 

## <a name="types-of-extended-properties"></a><span data-ttu-id="26e05-117">拡張プロパティのタイプ</span><span class="sxs-lookup"><span data-stu-id="26e05-117">Types of extended properties</span></span>

<span data-ttu-id="26e05-118">拡張プロパティに単一の値を保存するか、または (同じ型の) 複数の値を保存するかに応じて、拡張プロパティを [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md)、または [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) として作成できます。</span><span class="sxs-lookup"><span data-stu-id="26e05-118">Depending on whether you intend to store a single or multiple values (of the same type) in an extended property, you can create an extended property as a [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md), or [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md).</span></span>

<span data-ttu-id="26e05-119">これらのタイプはそれぞれ、**id** によってプロパティを識別し、データを **value** に格納します。</span><span class="sxs-lookup"><span data-stu-id="26e05-119">Each of these types identifies the property by its **id** and stores data in **value**.</span></span> 

<span data-ttu-id="26e05-120">**id** を使用して、特定のリソース インスタンスをその拡張プロパティと一緒に取得するか、単一の値の拡張プロパティでフィルターして、そのプロパティのすべてのインスタンスを取得できます。</span><span class="sxs-lookup"><span data-stu-id="26e05-120">You can use **id** to get a specific resource instance together with that extended property, or filter on a single-value extended property to get all the instances that have that property.</span></span> 

<span data-ttu-id="26e05-121">**注** REST API を使用して、1 つの呼び出しで特定のインスタンスのすべての拡張プロパティを取得することはできません。</span><span class="sxs-lookup"><span data-stu-id="26e05-121">**Note** You cannot use the REST API to get all the extended properties of a specific instance in one call.</span></span>
  

### <a name="id-formats"></a><span data-ttu-id="26e05-122">id の形式</span><span class="sxs-lookup"><span data-stu-id="26e05-122">id Formats</span></span>

<span data-ttu-id="26e05-123">単一値または複数値の拡張プロパティを作成する場合、文字列の名前 (**Name**) または数値識別子 (**Id**) のいずれか、および値の実際の型またはプロパティの値に基づき、2 つの形式のいずれかで **id** プロパティを指定できます。</span><span class="sxs-lookup"><span data-stu-id="26e05-123">When creating a single-value or multi-value extended property, you can specify the **PropertyId** in one of two formats, based on either a string name or numeric identifier, and on the actual type of value or values of the property.</span></span> <span data-ttu-id="26e05-124">以下に示す 2 つの表では、単一値または複数値の拡張プロパティを指定するためにサポートされている形式について説明します。</span><span class="sxs-lookup"><span data-stu-id="26e05-124">The next 2 tables below describe the supported formats to specify single and multi-value extended properties.</span></span> <span data-ttu-id="26e05-125">{_type_} はプロパティ値の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="26e05-125">{_type_} represents the type of the value or values of the property.</span></span> <span data-ttu-id="26e05-126">この例では、文字列、整数、およびこれらの種類の配列を示しています。</span><span class="sxs-lookup"><span data-stu-id="26e05-126">Shown in the examples are string, integer, and arrays of these types.</span></span>

<span data-ttu-id="26e05-127">拡張プロパティはほとんどの場合、Microsoft Graph API メタデータで公開されていない定義済みの MAPI プロパティと相互運用します。したがって、簡略化のため、選択する形式は、対応する MAPI プロパティが [MAPI プロパティの識別子]((https://msdn.microsoft.com/ja-JP/library/office/cc815528.aspx))で文字列を使用しているか、数値を使用しているかを反映する必要があります。</span><span class="sxs-lookup"><span data-stu-id="26e05-127">Since extended properties are in most cases inter-operating with defined MAPI properties not exposed in the Outlook REST API metadata, for simplicity, the format you choose should reflect whether the corresponding MAPI property uses a character string or numeric value in its [MAPI property identifier]((https://msdn.microsoft.com/ja-JP/library/office/cc815528.aspx)).</span></span>
<span data-ttu-id="26e05-128">
  \[MS-OXPROPS\] Microsoft Corporation の[「Exchange Server プロトコルのマスター プロパティ リスト」](https://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx)では、既存の MAPI プロパティへの拡張プロパティのマッピングに関する情報 (プロパティ識別子や GUID など) を検索できます。</span><span class="sxs-lookup"><span data-stu-id="26e05-128">You can find information that you would need to map an extended property to an existing MAPI property, such as the property identifier and GUID, in \[MS-OXPROPS\] Microsoft Corporation, ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx).</span></span>

<span data-ttu-id="26e05-129">**注** **id** に対して 1 つの形式を選択したら、その形式でのみ拡張プロパティにアクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="26e05-129">**Note** After you have chosen one format for the **id**, you should access that extended property by only that format.</span></span>


<span data-ttu-id="26e05-130">**単一値の拡張プロパティに有効な id の形式**</span><span class="sxs-lookup"><span data-stu-id="26e05-130">**Valid id formats for single-value extended properties**</span></span>

|<span data-ttu-id="26e05-131">**形式**</span><span class="sxs-lookup"><span data-stu-id="26e05-131">**Format**</span></span>|<span data-ttu-id="26e05-132">**例**</span><span class="sxs-lookup"><span data-stu-id="26e05-132">**Example**</span></span>|<span data-ttu-id="26e05-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="26e05-133">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="26e05-134">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="26e05-134">"{type} {guid} Name {name}"</span></span> | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="26e05-135">属している名前空間 (GUID) と名前で、プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="26e05-135">Identifies a property by the namespace (the GUID) it belongs to, and a name.</span></span>         |
| <span data-ttu-id="26e05-136">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="26e05-136">"{type} {guid} Id {id}"</span></span>     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | <span data-ttu-id="26e05-137">属している名前空間 (GUID) と識別子で、プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="26e05-137">Identifies a property by the namespace (the GUID) it belongs to, and an identifier.</span></span>  |

<span data-ttu-id="26e05-138">**複数値の拡張プロパティに有効な id の形式**</span><span class="sxs-lookup"><span data-stu-id="26e05-138">**Valid id formats for multi-value extended properties**</span></span>

|<span data-ttu-id="26e05-139">**形式**</span><span class="sxs-lookup"><span data-stu-id="26e05-139">**Format**</span></span>|<span data-ttu-id="26e05-140">**例**</span><span class="sxs-lookup"><span data-stu-id="26e05-140">**Example**</span></span>|<span data-ttu-id="26e05-141">**説明**</span><span class="sxs-lookup"><span data-stu-id="26e05-141">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="26e05-142">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="26e05-142">"{type} {guid} Name {name}"</span></span> | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="26e05-143">名前空間 (GUID) と名前で、プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="26e05-143">Identifies a property by namespace (the GUID) and name.</span></span>         |
| <span data-ttu-id="26e05-144">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="26e05-144">"{type} {guid} Id {id}"</span></span>     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | <span data-ttu-id="26e05-145">名前空間 (GUID) と識別子で、プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="26e05-145">Identifies a property by namespace (the GUID) and identifier.</span></span>   |

### <a name="rest-api-operations"></a><span data-ttu-id="26e05-146">REST API の操作</span><span class="sxs-lookup"><span data-stu-id="26e05-146">REST API operations</span></span>
 
<span data-ttu-id="26e05-147">単一値の拡張プロパティの操作:</span><span class="sxs-lookup"><span data-stu-id="26e05-147">Single-value extended property operations:</span></span>

- [<span data-ttu-id="26e05-148">新規または既存のリソースのインスタンスに、拡張プロパティを作成します</span><span class="sxs-lookup"><span data-stu-id="26e05-148">Create an extended property in a new or existing resource instance</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md)
- [<span data-ttu-id="26e05-149">`$expand` または `$filter` を使用し、拡張プロパティを含むリソース インスタンスを 1 つまたはコレクションで取得します</span><span class="sxs-lookup"><span data-stu-id="26e05-149">Get one or a collection of resource instances with an extended property using `$expand` or `$filter`</span></span>](../api/singlevaluelegacyextendedproperty_get.md)

<span data-ttu-id="26e05-150">複数値の拡張プロパティの操作:</span><span class="sxs-lookup"><span data-stu-id="26e05-150">Multi-value extended property operations:</span></span>

- [<span data-ttu-id="26e05-151">新規または既存のリソースのインスタンスに、拡張プロパティを作成します</span><span class="sxs-lookup"><span data-stu-id="26e05-151">Create an extended property in a new or existing resource instance</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md)
- [<span data-ttu-id="26e05-152">`$expand` を使用して拡張プロパティを含むリソース インスタンスを取得します</span><span class="sxs-lookup"><span data-stu-id="26e05-152">Get a resource instance with an extended property using `$expand`</span></span>](../api/multivaluelegacyextendedproperty_get.md)

