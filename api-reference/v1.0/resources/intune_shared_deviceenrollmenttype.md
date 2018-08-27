# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="7a66b-101">deviceEnrollmentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="7a66b-101">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="7a66b-102">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7a66b-102">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a66b-103">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a66b-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a66b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7a66b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a66b-105">管理するモバイル デバイスを追加するための方法です。</span><span class="sxs-lookup"><span data-stu-id="7a66b-105">Possible ways of adding a mobile device to management.</span></span>
## <a name="members"></a><span data-ttu-id="7a66b-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="7a66b-106">Members</span></span>
|<span data-ttu-id="7a66b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="7a66b-107">Member</span></span>|<span data-ttu-id="7a66b-108">値</span><span class="sxs-lookup"><span data-stu-id="7a66b-108">Value</span></span>|<span data-ttu-id="7a66b-109">説明</span><span class="sxs-lookup"><span data-stu-id="7a66b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a66b-110">不明</span><span class="sxs-lookup"><span data-stu-id="7a66b-110">unknown</span></span>|<span data-ttu-id="7a66b-111">0</span><span class="sxs-lookup"><span data-stu-id="7a66b-111">0%</span></span>|<span data-ttu-id="7a66b-112">登録型の既定値は収集されませんでした。</span><span class="sxs-lookup"><span data-stu-id="7a66b-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="7a66b-113">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="7a66b-113">userEnrollment</span></span>|<span data-ttu-id="7a66b-114">1</span><span class="sxs-lookup"><span data-stu-id="7a66b-114">-1</span></span>|<span data-ttu-id="7a66b-115">BYOD チャネルを通じてユーザー駆動の登録を行います。</span><span class="sxs-lookup"><span data-stu-id="7a66b-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="7a66b-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="7a66b-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="7a66b-117">2</span><span class="sxs-lookup"><span data-stu-id="7a66b-117">-2</span></span>|<span data-ttu-id="7a66b-118">デバイス登録の管理者アカウントでユーザーを登録します。</span><span class="sxs-lookup"><span data-stu-id="7a66b-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="7a66b-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="7a66b-119">appleBulkWithUser</span></span>|<span data-ttu-id="7a66b-120">3</span><span class="sxs-lookup"><span data-stu-id="7a66b-120">"3"</span></span>|<span data-ttu-id="7a66b-121">ユーザーチャレンジを使って Apple の一括登録を行います。</span><span class="sxs-lookup"><span data-stu-id="7a66b-121">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="7a66b-122">(DEP、Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="7a66b-122">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="7a66b-123">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="7a66b-123">appleBulkWithoutUser</span></span>|<span data-ttu-id="7a66b-124">4</span><span class="sxs-lookup"><span data-stu-id="7a66b-124">-4</span></span>|<span data-ttu-id="7a66b-125">ユーザーチャレンジを使わないで Apple の一括登録を行います。</span><span class="sxs-lookup"><span data-stu-id="7a66b-125">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="7a66b-126">(DEP、Apple Configurator、モバイルコンフィギュレーター)</span><span class="sxs-lookup"><span data-stu-id="7a66b-126">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="7a66b-127">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="7a66b-127">windowsAzureADJoin</span></span>|<span data-ttu-id="7a66b-128">5</span><span class="sxs-lookup"><span data-stu-id="7a66b-128">.5</span></span>|<span data-ttu-id="7a66b-129">Windows 10 で Azure AD を参加させます。</span><span class="sxs-lookup"><span data-stu-id="7a66b-129">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="7a66b-130">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="7a66b-130">windowsBulkUserless</span></span>|<span data-ttu-id="7a66b-131">6</span><span class="sxs-lookup"><span data-stu-id="7a66b-131">-6</span></span>|<span data-ttu-id="7a66b-132">証明書を使って ICD から Windows 10 の一括登録を行います。</span><span class="sxs-lookup"><span data-stu-id="7a66b-132">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="7a66b-133">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="7a66b-133">windowsAutoEnrollment</span></span>|<span data-ttu-id="7a66b-134">7</span><span class="sxs-lookup"><span data-stu-id="7a66b-134">-7</span></span>|<span data-ttu-id="7a66b-135">Windows 10 自動登録です。</span><span class="sxs-lookup"><span data-stu-id="7a66b-135">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="7a66b-136">(勤務先のアカウントを追加)</span><span class="sxs-lookup"><span data-stu-id="7a66b-136">(Add work account)</span></span>|
|<span data-ttu-id="7a66b-137">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="7a66b-137">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="7a66b-138">8</span><span class="sxs-lookup"><span data-stu-id="7a66b-138">-8</span></span>|<span data-ttu-id="7a66b-139">Windows 10 で Azure AD を一括参加させます。</span><span class="sxs-lookup"><span data-stu-id="7a66b-139">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="7a66b-140">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="7a66b-140">windowsCoManagement</span></span>|<span data-ttu-id="7a66b-141">9</span><span class="sxs-lookup"><span data-stu-id="7a66b-141">-9</span></span>|<span data-ttu-id="7a66b-142">Windows 10 共同管理が AutoPilot またはグループ ポリシーによって起動します。</span><span class="sxs-lookup"><span data-stu-id="7a66b-142">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|


