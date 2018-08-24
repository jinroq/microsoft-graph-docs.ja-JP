# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="ef148-101">mobileAppPublishingState 列挙型</span><span class="sxs-lookup"><span data-stu-id="ef148-101">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="ef148-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ef148-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef148-103">アプリの公開状態を示します。</span><span class="sxs-lookup"><span data-stu-id="ef148-103">Indicates the publishing state of an app.</span></span>
## <a name="members"></a><span data-ttu-id="ef148-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="ef148-104">Members</span></span>
|<span data-ttu-id="ef148-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="ef148-105">Member</span></span>|<span data-ttu-id="ef148-106">値</span><span class="sxs-lookup"><span data-stu-id="ef148-106">Value</span></span>|<span data-ttu-id="ef148-107">説明</span><span class="sxs-lookup"><span data-stu-id="ef148-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef148-108">notPublished</span><span class="sxs-lookup"><span data-stu-id="ef148-108">notPublished</span></span>|<span data-ttu-id="ef148-109">0</span><span class="sxs-lookup"><span data-stu-id="ef148-109">0%</span></span>|<span data-ttu-id="ef148-110">アプリは公開されていません。</span><span class="sxs-lookup"><span data-stu-id="ef148-110">The app is not yet published.</span></span>|
|<span data-ttu-id="ef148-111">processing</span><span class="sxs-lookup"><span data-stu-id="ef148-111">processing</span></span>|<span data-ttu-id="ef148-112">1</span><span class="sxs-lookup"><span data-stu-id="ef148-112">-1</span></span>|<span data-ttu-id="ef148-113">アプリはサービス側の処理を保留しています。</span><span class="sxs-lookup"><span data-stu-id="ef148-113">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="ef148-114">published</span><span class="sxs-lookup"><span data-stu-id="ef148-114">published</span></span>|<span data-ttu-id="ef148-115">2</span><span class="sxs-lookup"><span data-stu-id="ef148-115">-2</span></span>|<span data-ttu-id="ef148-116">アプリは公開されています。</span><span class="sxs-lookup"><span data-stu-id="ef148-116">The app is removed.</span></span>|



