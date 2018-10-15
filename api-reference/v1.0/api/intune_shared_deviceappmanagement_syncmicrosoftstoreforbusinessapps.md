# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="028c0-101">syncMicrosoftStoreForBusinessApps アクション</span><span class="sxs-lookup"><span data-stu-id="028c0-101">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="028c0-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="028c0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="028c0-103">ビジネス向け Microsoft Store と Intune アカウントを同期する</span><span class="sxs-lookup"><span data-stu-id="028c0-103">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="028c0-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="028c0-104">Prerequisites</span></span>
<span data-ttu-id="028c0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="028c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="028c0-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="028c0-107">Permission type</span></span>|<span data-ttu-id="028c0-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="028c0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="028c0-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="028c0-109">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="028c0-110">&nbsp; &nbsp; _新人研修_</span><span class="sxs-lookup"><span data-stu-id="028c0-110">&nbsp; &nbsp; _On-boarding_</span></span> | <span data-ttu-id="028c0-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="028c0-111">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="028c0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="028c0-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="028c0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="028c0-113">Not supported.</span></span>|
|<span data-ttu-id="028c0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="028c0-114">Application</span></span>|<span data-ttu-id="028c0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="028c0-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="028c0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="028c0-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="028c0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="028c0-117">Request headers</span></span>
|<span data-ttu-id="028c0-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="028c0-118">Header</span></span>|<span data-ttu-id="028c0-119">値</span><span class="sxs-lookup"><span data-stu-id="028c0-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="028c0-120">承認</span><span class="sxs-lookup"><span data-stu-id="028c0-120">Authorization</span></span>|<span data-ttu-id="028c0-121">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="028c0-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="028c0-122">承諾</span><span class="sxs-lookup"><span data-stu-id="028c0-122">Accept</span></span>|<span data-ttu-id="028c0-123">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="028c0-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="028c0-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="028c0-124">Request body</span></span>
<span data-ttu-id="028c0-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="028c0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="028c0-126">応答</span><span class="sxs-lookup"><span data-stu-id="028c0-126">Response</span></span>
<span data-ttu-id="028c0-127">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="028c0-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="028c0-128">要求の例</span><span class="sxs-lookup"><span data-stu-id="028c0-128">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="028c0-129">応答</span><span class="sxs-lookup"><span data-stu-id="028c0-129">Response</span></span>

<span data-ttu-id="028c0-130">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="028c0-130">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="028c0-131">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="028c0-131">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



