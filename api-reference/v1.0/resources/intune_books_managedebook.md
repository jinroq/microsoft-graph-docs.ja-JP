# <a name="managedebook-resource-type"></a><span data-ttu-id="4d99c-101">managedEBook リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4d99c-101">managedEBook resource type</span></span>

> <span data-ttu-id="4d99c-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4d99c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d99c-103">管理対象電子ブックの基本プロパティを含む抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="4d99c-103">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="4d99c-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="4d99c-104">Methods</span></span>
|<span data-ttu-id="4d99c-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="4d99c-105">Method</span></span>|<span data-ttu-id="4d99c-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4d99c-106">Return Type</span></span>|<span data-ttu-id="4d99c-107">説明</span><span class="sxs-lookup"><span data-stu-id="4d99c-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4d99c-108">managedEBook のリスト</span><span class="sxs-lookup"><span data-stu-id="4d99c-108">List managedEBooks</span></span>](../api/intune_books_managedebook_list.md)|<span data-ttu-id="4d99c-109">[managedEBook](../resources/intune_books_managedebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4d99c-109">[managedEBook](../resources/intune_books_managedebook.md) collection</span></span>|<span data-ttu-id="4d99c-110">[managedEBook](../resources/intune_books_managedebook.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4d99c-110">List properties and relationships of the [managedEBook](../resources/intune_books_managedebook.md) objects.</span></span>|
|[<span data-ttu-id="4d99c-111">managedEBook の取得</span><span class="sxs-lookup"><span data-stu-id="4d99c-111">Get managedEBook</span></span>](../api/intune_books_managedebook_get.md)|[<span data-ttu-id="4d99c-112">managedEBook</span><span class="sxs-lookup"><span data-stu-id="4d99c-112">managedEBook</span></span>](../resources/intune_books_managedebook.md)|<span data-ttu-id="4d99c-113">[managedEBook](../resources/intune_books_managedebook.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4d99c-113">Read properties and relationships of the [managedEBook](../resources/intune_books_managedebook.md) object.</span></span>|
|[<span data-ttu-id="4d99c-114">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="4d99c-114">assign action</span></span>](../api/intune_books_managedebook_assign.md)|<span data-ttu-id="4d99c-115">なし</span><span class="sxs-lookup"><span data-stu-id="4d99c-115">None</span></span>|<span data-ttu-id="4d99c-116">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4d99c-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="4d99c-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d99c-117">Properties</span></span>
|<span data-ttu-id="4d99c-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d99c-118">Property</span></span>|<span data-ttu-id="4d99c-119">タイプ</span><span class="sxs-lookup"><span data-stu-id="4d99c-119">Type</span></span>|<span data-ttu-id="4d99c-120">説明</span><span class="sxs-lookup"><span data-stu-id="4d99c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d99c-121">ID</span><span class="sxs-lookup"><span data-stu-id="4d99c-121">id</span></span>|<span data-ttu-id="4d99c-122">文字列</span><span class="sxs-lookup"><span data-stu-id="4d99c-122">String</span></span>|<span data-ttu-id="4d99c-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4d99c-123">Key of the entity.</span></span>|
|<span data-ttu-id="4d99c-124">displayName</span><span class="sxs-lookup"><span data-stu-id="4d99c-124">displayName</span></span>|<span data-ttu-id="4d99c-125">文字列</span><span class="sxs-lookup"><span data-stu-id="4d99c-125">String</span></span>|<span data-ttu-id="4d99c-126">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="4d99c-126">Name of the eBook.</span></span>|
|<span data-ttu-id="4d99c-127">説明</span><span class="sxs-lookup"><span data-stu-id="4d99c-127">description</span></span>|<span data-ttu-id="4d99c-128">文字列</span><span class="sxs-lookup"><span data-stu-id="4d99c-128">String</span></span>|<span data-ttu-id="4d99c-129">説明。</span><span class="sxs-lookup"><span data-stu-id="4d99c-129">Description.</span></span>|
|<span data-ttu-id="4d99c-130">パブリッシャー</span><span class="sxs-lookup"><span data-stu-id="4d99c-130">publisher</span></span>|<span data-ttu-id="4d99c-131">文字列</span><span class="sxs-lookup"><span data-stu-id="4d99c-131">String</span></span>|<span data-ttu-id="4d99c-132">発行元です。</span><span class="sxs-lookup"><span data-stu-id="4d99c-132">Publisher.</span></span>|
|<span data-ttu-id="4d99c-133">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d99c-133">publishedDateTime</span></span>|<span data-ttu-id="4d99c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d99c-134">DateTimeOffset</span></span>|<span data-ttu-id="4d99c-135">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="4d99c-135">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="4d99c-136">大型カバー</span><span class="sxs-lookup"><span data-stu-id="4d99c-136">largeCover</span></span>|[<span data-ttu-id="4d99c-137">マイムコンテンツ</span><span class="sxs-lookup"><span data-stu-id="4d99c-137">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="4d99c-138">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="4d99c-138">Book cover.</span></span>|
|<span data-ttu-id="4d99c-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4d99c-139">createdDateTime</span></span>|<span data-ttu-id="4d99c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d99c-140">DateTimeOffset</span></span>|<span data-ttu-id="4d99c-141">電子ブック ファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="4d99c-141">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="4d99c-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d99c-142">lastModifiedDateTime</span></span>|<span data-ttu-id="4d99c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d99c-143">DateTimeOffset</span></span>|<span data-ttu-id="4d99c-144">電子ブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="4d99c-144">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="4d99c-145">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4d99c-145">informationUrl</span></span>|<span data-ttu-id="4d99c-146">文字列</span><span class="sxs-lookup"><span data-stu-id="4d99c-146">String</span></span>|<span data-ttu-id="4d99c-147">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="4d99c-147">The more information Url.</span></span>|
|<span data-ttu-id="4d99c-148">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4d99c-148">privacyInformationUrl</span></span>|<span data-ttu-id="4d99c-149">文字列</span><span class="sxs-lookup"><span data-stu-id="4d99c-149">String</span></span>|<span data-ttu-id="4d99c-150">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="4d99c-150">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d99c-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4d99c-151">Relationships</span></span>
|<span data-ttu-id="4d99c-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4d99c-152">Relationship</span></span>|<span data-ttu-id="4d99c-153">型</span><span class="sxs-lookup"><span data-stu-id="4d99c-153">Type</span></span>|<span data-ttu-id="4d99c-154">説明</span><span class="sxs-lookup"><span data-stu-id="4d99c-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d99c-155">割り当て</span><span class="sxs-lookup"><span data-stu-id="4d99c-155">assignments</span></span>|<span data-ttu-id="4d99c-156">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4d99c-156">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) collection</span></span>|<span data-ttu-id="4d99c-157">この電子ブックの割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="4d99c-157">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="4d99c-158">installSummary</span><span class="sxs-lookup"><span data-stu-id="4d99c-158">installSummary</span></span>|[<span data-ttu-id="4d99c-159">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="4d99c-159">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="4d99c-160">モバイル アプリ インストール概要です。</span><span class="sxs-lookup"><span data-stu-id="4d99c-160">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="4d99c-161">deviceStates</span><span class="sxs-lookup"><span data-stu-id="4d99c-161">deviceStates</span></span>|<span data-ttu-id="4d99c-162">[deviceInstallState](../resources/intune_books_deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4d99c-162">[deviceInstallState](../resources/intune_books_deviceinstallstate.md) collection</span></span>|<span data-ttu-id="4d99c-163">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="4d99c-163">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="4d99c-164">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="4d99c-164">userStateSummary</span></span>|<span data-ttu-id="4d99c-165">[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4d99c-165">[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="4d99c-166">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="4d99c-166">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d99c-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4d99c-167">JSON Representation</span></span>
<span data-ttu-id="4d99c-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4d99c-168">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}-->
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








