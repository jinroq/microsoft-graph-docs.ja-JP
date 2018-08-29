# <a name="intunebrand-resource-type"></a><span data-ttu-id="93ef9-101">intuneBrand リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="93ef9-101">intuneBrand resource type</span></span>

> <span data-ttu-id="93ef9-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="93ef9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93ef9-103">intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="93ef9-103">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>
## <a name="properties"></a><span data-ttu-id="93ef9-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93ef9-104">Properties</span></span>
|<span data-ttu-id="93ef9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93ef9-105">Property</span></span>|<span data-ttu-id="93ef9-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="93ef9-106">Type</span></span>|<span data-ttu-id="93ef9-107">説明</span><span class="sxs-lookup"><span data-stu-id="93ef9-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93ef9-108">displayName</span><span class="sxs-lookup"><span data-stu-id="93ef9-108">displayName</span></span>|<span data-ttu-id="93ef9-109">String</span><span class="sxs-lookup"><span data-stu-id="93ef9-109">String</span></span>|<span data-ttu-id="93ef9-110">エンド ユーザーに表示される会社名または組織名。</span><span class="sxs-lookup"><span data-stu-id="93ef9-110">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="93ef9-111">contactITName</span><span class="sxs-lookup"><span data-stu-id="93ef9-111">contactITName</span></span>|<span data-ttu-id="93ef9-112">String</span><span class="sxs-lookup"><span data-stu-id="93ef9-112">String</span></span>|<span data-ttu-id="93ef9-113">IT サポートを担当する個人名または組織名。</span><span class="sxs-lookup"><span data-stu-id="93ef9-113">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="93ef9-114">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="93ef9-114">contactITPhoneNumber</span></span>|<span data-ttu-id="93ef9-115">String</span><span class="sxs-lookup"><span data-stu-id="93ef9-115">String</span></span>|<span data-ttu-id="93ef9-116">IT サポートを担当する個人または組織の電話番号。</span><span class="sxs-lookup"><span data-stu-id="93ef9-116">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="93ef9-117">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="93ef9-117">contactITEmailAddress</span></span>|<span data-ttu-id="93ef9-118">String</span><span class="sxs-lookup"><span data-stu-id="93ef9-118">String</span></span>|<span data-ttu-id="93ef9-119">IT サポートを担当する個人または組織のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="93ef9-119">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="93ef9-120">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="93ef9-120">contactITNotes</span></span>|<span data-ttu-id="93ef9-121">String</span><span class="sxs-lookup"><span data-stu-id="93ef9-121">String</span></span>|<span data-ttu-id="93ef9-122">IT サポートを担当する個人または組織に関するテキスト コメント。</span><span class="sxs-lookup"><span data-stu-id="93ef9-122">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="93ef9-123">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="93ef9-123">privacyUrl</span></span>|<span data-ttu-id="93ef9-124">String</span><span class="sxs-lookup"><span data-stu-id="93ef9-124">String</span></span>|<span data-ttu-id="93ef9-125">会社または組織のプライバシー ポリシーの URL。</span><span class="sxs-lookup"><span data-stu-id="93ef9-125">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="93ef9-126">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="93ef9-126">onlineSupportSiteUrl</span></span>|<span data-ttu-id="93ef9-127">String</span><span class="sxs-lookup"><span data-stu-id="93ef9-127">String</span></span>|<span data-ttu-id="93ef9-128">会社または組織の IT ヘルプデスク サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="93ef9-128">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="93ef9-129">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="93ef9-129">onlineSupportSiteName</span></span>|<span data-ttu-id="93ef9-130">String</span><span class="sxs-lookup"><span data-stu-id="93ef9-130">String</span></span>|<span data-ttu-id="93ef9-131">会社または組織の IT ヘルプデスク サイトの表示名。</span><span class="sxs-lookup"><span data-stu-id="93ef9-131">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="93ef9-132">themeColor</span><span class="sxs-lookup"><span data-stu-id="93ef9-132">themeColor</span></span>|[<span data-ttu-id="93ef9-133">rgbColor</span><span class="sxs-lookup"><span data-stu-id="93ef9-133">rgbColor</span></span>](../resources/intune_onboarding_rgbcolor.md)|<span data-ttu-id="93ef9-134">会社のポータル アプリケーションと Web ポータルで使用する主要なテーマの色。</span><span class="sxs-lookup"><span data-stu-id="93ef9-134">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="93ef9-135">showLogo</span><span class="sxs-lookup"><span data-stu-id="93ef9-135">showLogo</span></span>|<span data-ttu-id="93ef9-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="93ef9-136">Boolean</span></span>|<span data-ttu-id="93ef9-137">管理者が指定したロゴ画像が表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="93ef9-137">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="93ef9-138">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="93ef9-138">lightBackgroundLogo</span></span>|[<span data-ttu-id="93ef9-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="93ef9-139">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="93ef9-140">ロゴの背景色が明るいポータル サイト アプリに表示されるロゴ画像。</span><span class="sxs-lookup"><span data-stu-id="93ef9-140">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="93ef9-141">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="93ef9-141">darkBackgroundLogo</span></span>|[<span data-ttu-id="93ef9-142">mimeContent</span><span class="sxs-lookup"><span data-stu-id="93ef9-142">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="93ef9-143">ロゴの背景色が暗いポータル サイト アプリに表示されるロゴ画像。</span><span class="sxs-lookup"><span data-stu-id="93ef9-143">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="93ef9-144">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="93ef9-144">showNameNextToLogo</span></span>|<span data-ttu-id="93ef9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="93ef9-145">Boolean</span></span>|<span data-ttu-id="93ef9-146">管理者が指定した名前がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="93ef9-146">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="93ef9-147">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="93ef9-147">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="93ef9-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="93ef9-148">Boolean</span></span>|<span data-ttu-id="93ef9-149">管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="93ef9-149">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93ef9-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="93ef9-150">Relationships</span></span>
<span data-ttu-id="93ef9-151">なし</span><span class="sxs-lookup"><span data-stu-id="93ef9-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="93ef9-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="93ef9-152">JSON Representation</span></span>
<span data-ttu-id="93ef9-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="93ef9-153">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "privacyUrl": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showNameNextToLogo": true,
  "showDisplayNameNextToLogo": true
}
```



