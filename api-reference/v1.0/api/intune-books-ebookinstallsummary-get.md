---
title: Get eBookInstallSummary
description: eBookInstallSummary オブジェクトのプロパティとリレーションシップを読み取ります。
ms.openlocfilehash: 6bde238d86605d4568cd43879bebbf4ad8768233
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023575"
---
# <a name="get-ebookinstallsummary"></a><span data-ttu-id="79b9d-103">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="79b9d-103">Get eBookInstallSummary</span></span>

> <span data-ttu-id="79b9d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="79b9d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79b9d-105">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="79b9d-105">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79b9d-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="79b9d-106">Prerequisites</span></span>
<span data-ttu-id="79b9d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79b9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79b9d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79b9d-109">Permission type</span></span>|<span data-ttu-id="79b9d-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="79b9d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79b9d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79b9d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="79b9d-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="79b9d-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="79b9d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79b9d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79b9d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79b9d-114">Not supported.</span></span>|
|<span data-ttu-id="79b9d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79b9d-115">Application</span></span>|<span data-ttu-id="79b9d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79b9d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79b9d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79b9d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79b9d-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="79b9d-118">Optional query parameters</span></span>
<span data-ttu-id="79b9d-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="79b9d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="79b9d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79b9d-120">Request headers</span></span>
|<span data-ttu-id="79b9d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79b9d-121">Header</span></span>|<span data-ttu-id="79b9d-122">値</span><span class="sxs-lookup"><span data-stu-id="79b9d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79b9d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79b9d-123">Authorization</span></span>|<span data-ttu-id="79b9d-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="79b9d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79b9d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="79b9d-125">Accept</span></span>|<span data-ttu-id="79b9d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79b9d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79b9d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="79b9d-127">Request body</span></span>
<span data-ttu-id="79b9d-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="79b9d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79b9d-129">応答</span><span class="sxs-lookup"><span data-stu-id="79b9d-129">Response</span></span>
<span data-ttu-id="79b9d-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="79b9d-130">If successful, this method returns a `200 OK` response code and [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79b9d-131">例</span><span class="sxs-lookup"><span data-stu-id="79b9d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="79b9d-132">要求</span><span class="sxs-lookup"><span data-stu-id="79b9d-132">Request</span></span>
<span data-ttu-id="79b9d-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79b9d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

### <a name="response"></a><span data-ttu-id="79b9d-134">応答</span><span class="sxs-lookup"><span data-stu-id="79b9d-134">Response</span></span>
<span data-ttu-id="79b9d-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79b9d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 320

{
  "value": {
    "@odata.type": "#microsoft.graph.eBookInstallSummary",
    "id": "9708ad78-ad78-9708-78ad-089778ad0897",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7,
    "installedUserCount": 2,
    "failedUserCount": 15,
    "notInstalledUserCount": 5
  }
}
```


