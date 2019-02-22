---
title: Get userInstallStateSummary
description: userInstallStateSummary オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 28887461c57b6b195c5a80330f35b337946126e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145487"
---
# <a name="get-userinstallstatesummary"></a><span data-ttu-id="46224-103">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="46224-103">Get userInstallStateSummary</span></span>

> <span data-ttu-id="46224-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46224-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46224-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="46224-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46224-106">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="46224-106">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46224-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="46224-107">Prerequisites</span></span>
<span data-ttu-id="46224-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46224-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="46224-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="46224-110">Permission type</span></span>|<span data-ttu-id="46224-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="46224-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46224-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="46224-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46224-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="46224-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="46224-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="46224-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46224-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46224-115">Not supported.</span></span>|
|<span data-ttu-id="46224-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="46224-116">Application</span></span>|<span data-ttu-id="46224-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46224-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46224-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="46224-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46224-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="46224-119">Optional query parameters</span></span>
<span data-ttu-id="46224-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="46224-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46224-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46224-121">Request headers</span></span>
|<span data-ttu-id="46224-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46224-122">Header</span></span>|<span data-ttu-id="46224-123">値</span><span class="sxs-lookup"><span data-stu-id="46224-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46224-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="46224-124">Authorization</span></span>|<span data-ttu-id="46224-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="46224-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46224-126">承諾</span><span class="sxs-lookup"><span data-stu-id="46224-126">Accept</span></span>|<span data-ttu-id="46224-127">application/json</span><span class="sxs-lookup"><span data-stu-id="46224-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46224-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="46224-128">Request body</span></span>
<span data-ttu-id="46224-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="46224-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46224-130">応答</span><span class="sxs-lookup"><span data-stu-id="46224-130">Response</span></span>
<span data-ttu-id="46224-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="46224-131">If successful, this method returns a `200 OK` response code and [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46224-132">例</span><span class="sxs-lookup"><span data-stu-id="46224-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="46224-133">要求</span><span class="sxs-lookup"><span data-stu-id="46224-133">Request</span></span>
<span data-ttu-id="46224-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="46224-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="46224-135">応答</span><span class="sxs-lookup"><span data-stu-id="46224-135">Response</span></span>
<span data-ttu-id="46224-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="46224-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




