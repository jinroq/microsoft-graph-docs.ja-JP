# <a name="managedebook-resource-type"></a><span data-ttu-id="6a4f6-101">managedEBook リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6a4f6-101">managedEBook resource type</span></span>

> <span data-ttu-id="6a4f6-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a4f6-103">管理対象電子ブックの基本プロパティを含む抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-103">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="6a4f6-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="6a4f6-104">Methods</span></span>
|<span data-ttu-id="6a4f6-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="6a4f6-105">Method</span></span>|<span data-ttu-id="6a4f6-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6a4f6-106">Return Type</span></span>|<span data-ttu-id="6a4f6-107">説明</span><span class="sxs-lookup"><span data-stu-id="6a4f6-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6a4f6-108">managedEBooks のリスト</span><span class="sxs-lookup"><span data-stu-id="6a4f6-108">List managedEBooks</span></span>](../api/intune_books_managedebook_list.md)|<span data-ttu-id="6a4f6-109">[managedEBook](../resources/intune_books_managedebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6a4f6-109">[managedEBook](../resources/intune_books_managedebook.md) collection</span></span>|<span data-ttu-id="6a4f6-110">[managedEBook](../resources/intune_books_managedebook.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-110">List properties and relationships of the [managedEBook](../resources/intune_books_managedebook.md) objects.</span></span>|
|[<span data-ttu-id="6a4f6-111">managedEBook の取得</span><span class="sxs-lookup"><span data-stu-id="6a4f6-111">Get managedEBook</span></span>](../api/intune_books_managedebook_get.md)|[<span data-ttu-id="6a4f6-112">managedEBook</span><span class="sxs-lookup"><span data-stu-id="6a4f6-112">managedEBook</span></span>](../resources/intune_books_managedebook.md)|<span data-ttu-id="6a4f6-113">[managedEBook](../resources/intune_books_managedebook.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_books_managedebook.md) object.</span></span>|
|[<span data-ttu-id="6a4f6-114">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="6a4f6-114">assign action</span></span>](../api/intune_books_managedebook_assign.md)|<span data-ttu-id="6a4f6-115">なし</span><span class="sxs-lookup"><span data-stu-id="6a4f6-115">None</span></span>|<span data-ttu-id="6a4f6-116">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6a4f6-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6a4f6-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a4f6-117">Properties</span></span>
|<span data-ttu-id="6a4f6-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a4f6-118">Property</span></span>|<span data-ttu-id="6a4f6-119">型</span><span class="sxs-lookup"><span data-stu-id="6a4f6-119">Type</span></span>|<span data-ttu-id="6a4f6-120">説明</span><span class="sxs-lookup"><span data-stu-id="6a4f6-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a4f6-121">id</span><span class="sxs-lookup"><span data-stu-id="6a4f6-121">id</span></span>|<span data-ttu-id="6a4f6-122">String</span><span class="sxs-lookup"><span data-stu-id="6a4f6-122">String</span></span>|<span data-ttu-id="6a4f6-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-123">Name of the entity.</span></span>|
|<span data-ttu-id="6a4f6-124">displayName</span><span class="sxs-lookup"><span data-stu-id="6a4f6-124">displayName</span></span>|<span data-ttu-id="6a4f6-125">String</span><span class="sxs-lookup"><span data-stu-id="6a4f6-125">String</span></span>|<span data-ttu-id="6a4f6-126">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-126">Name of the folder.</span></span>|
|<span data-ttu-id="6a4f6-127">description</span><span class="sxs-lookup"><span data-stu-id="6a4f6-127">description</span></span>|<span data-ttu-id="6a4f6-128">String</span><span class="sxs-lookup"><span data-stu-id="6a4f6-128">String</span></span>|<span data-ttu-id="6a4f6-129">説明。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-129">Description.</span></span>|
|<span data-ttu-id="6a4f6-130">publisher</span><span class="sxs-lookup"><span data-stu-id="6a4f6-130">Publisher</span></span>|<span data-ttu-id="6a4f6-131">String</span><span class="sxs-lookup"><span data-stu-id="6a4f6-131">String</span></span>|<span data-ttu-id="6a4f6-132">発行元です。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-132">Publisher</span></span>|
|<span data-ttu-id="6a4f6-133">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a4f6-133">publishedDateTime</span></span>|<span data-ttu-id="6a4f6-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a4f6-134">DateTimeOffset</span></span>|<span data-ttu-id="6a4f6-135">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-135">The date and time when the page was created.</span></span>|
|<span data-ttu-id="6a4f6-136">largeCover</span><span class="sxs-lookup"><span data-stu-id="6a4f6-136">largeCover</span></span>|[<span data-ttu-id="6a4f6-137">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6a4f6-137">MimeContent</span></span>](../resources/intune_books_mimecontent.md)|<span data-ttu-id="6a4f6-138">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-138">Book cover</span></span>|
|<span data-ttu-id="6a4f6-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a4f6-139">createdDateTime</span></span>|<span data-ttu-id="6a4f6-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a4f6-140">DateTimeOffset</span></span>|<span data-ttu-id="6a4f6-141">電子ブック ファイルが作成された日時です。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-141">The date and time when the page was created.</span></span>|
|<span data-ttu-id="6a4f6-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a4f6-142">lastModifiedDateTime</span></span>|<span data-ttu-id="6a4f6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a4f6-143">DateTimeOffset</span></span>|<span data-ttu-id="6a4f6-144">電子ブックが最後に変更された日時です。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="6a4f6-145">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6a4f6-145">informationUrl</span></span>|<span data-ttu-id="6a4f6-146">String</span><span class="sxs-lookup"><span data-stu-id="6a4f6-146">String</span></span>|<span data-ttu-id="6a4f6-147">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-147">The more information Url.</span></span>|
|<span data-ttu-id="6a4f6-148">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6a4f6-148">privacyInformationUrl</span></span>|<span data-ttu-id="6a4f6-149">String</span><span class="sxs-lookup"><span data-stu-id="6a4f6-149">String</span></span>|<span data-ttu-id="6a4f6-150">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-150">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a4f6-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6a4f6-151">Relationships</span></span>
|<span data-ttu-id="6a4f6-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6a4f6-152">Relationship</span></span>|<span data-ttu-id="6a4f6-153">型</span><span class="sxs-lookup"><span data-stu-id="6a4f6-153">Type</span></span>|<span data-ttu-id="6a4f6-154">説明</span><span class="sxs-lookup"><span data-stu-id="6a4f6-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a4f6-155">assignments</span><span class="sxs-lookup"><span data-stu-id="6a4f6-155">assignments</span></span>|<span data-ttu-id="6a4f6-156">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6a4f6-156">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) collection</span></span>|<span data-ttu-id="6a4f6-157">この電子ブックの割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-157">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="6a4f6-158">installSummary</span><span class="sxs-lookup"><span data-stu-id="6a4f6-158">installSummary</span></span>|[<span data-ttu-id="6a4f6-159">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6a4f6-159">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="6a4f6-160">モバイル アプリ インストール概要です。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-160">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="6a4f6-161">deviceStates</span><span class="sxs-lookup"><span data-stu-id="6a4f6-161">deviceStates</span></span>|<span data-ttu-id="6a4f6-162">[deviceInstallState](../resources/intune_books_deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6a4f6-162">[deviceInstallState](../resources/intune_books_deviceinstallstate.md) collection</span></span>|<span data-ttu-id="6a4f6-163">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-163">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="6a4f6-164">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="6a4f6-164">userStateSummary</span></span>|<span data-ttu-id="6a4f6-165">[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6a4f6-165">[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="6a4f6-166">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-166">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a4f6-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6a4f6-167">JSON Representation</span></span>
<span data-ttu-id="6a4f6-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6a4f6-168">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```



