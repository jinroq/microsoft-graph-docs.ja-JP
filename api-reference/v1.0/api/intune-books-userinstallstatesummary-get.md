---
title: Get userInstallStateSummary
description: userInstallStateSummary オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
ms.openlocfilehash: 4d0506b9d0e4736479d6bdd70e4176ffd82ea87c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346607"
---
# <a name="get-userinstallstatesummary"></a><span data-ttu-id="c84cb-103">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="c84cb-103">Get userInstallStateSummary</span></span>

> <span data-ttu-id="c84cb-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c84cb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c84cb-105">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c84cb-105">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c84cb-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="c84cb-106">Prerequisites</span></span>
<span data-ttu-id="c84cb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c84cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c84cb-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c84cb-109">Permission type</span></span>|<span data-ttu-id="c84cb-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c84cb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c84cb-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c84cb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c84cb-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c84cb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c84cb-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c84cb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c84cb-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c84cb-114">Not supported.</span></span>|
|<span data-ttu-id="c84cb-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c84cb-115">Application</span></span>|<span data-ttu-id="c84cb-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c84cb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c84cb-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c84cb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c84cb-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c84cb-118">Optional query parameters</span></span>
<span data-ttu-id="c84cb-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c84cb-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c84cb-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c84cb-120">Request headers</span></span>
|<span data-ttu-id="c84cb-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c84cb-121">Header</span></span>|<span data-ttu-id="c84cb-122">値</span><span class="sxs-lookup"><span data-stu-id="c84cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c84cb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c84cb-123">Authorization</span></span>|<span data-ttu-id="c84cb-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c84cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c84cb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c84cb-125">Accept</span></span>|<span data-ttu-id="c84cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c84cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c84cb-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c84cb-127">Request body</span></span>
<span data-ttu-id="c84cb-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c84cb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c84cb-129">応答</span><span class="sxs-lookup"><span data-stu-id="c84cb-129">Response</span></span>
<span data-ttu-id="c84cb-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c84cb-130">If successful, this method returns a `200 OK` response code and [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c84cb-131">例</span><span class="sxs-lookup"><span data-stu-id="c84cb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c84cb-132">要求</span><span class="sxs-lookup"><span data-stu-id="c84cb-132">Request</span></span>
<span data-ttu-id="c84cb-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c84cb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="c84cb-134">応答</span><span class="sxs-lookup"><span data-stu-id="c84cb-134">Response</span></span>
<span data-ttu-id="c84cb-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c84cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "value": {
    "@odata.type": "#microsoft.graph.userInstallStateSummary",
    "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
    "userName": "User Name value",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7
  }
}
```



