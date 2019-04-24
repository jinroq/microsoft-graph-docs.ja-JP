---
title: リスト mobileAppDependencies
description: mobileAppDependency オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6fe13b2d62a9f5d4bffed4daf1f682dce33d7bc4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32489003"
---
# <a name="list-mobileappdependencies"></a><span data-ttu-id="b3a81-103">リスト mobileAppDependencies</span><span class="sxs-lookup"><span data-stu-id="b3a81-103">List mobileAppDependencies</span></span>

> <span data-ttu-id="b3a81-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3a81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3a81-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b3a81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3a81-106">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b3a81-106">List properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3a81-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b3a81-107">Prerequisites</span></span>
<span data-ttu-id="b3a81-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3a81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3a81-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b3a81-110">Permission type</span></span>|<span data-ttu-id="b3a81-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b3a81-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3a81-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b3a81-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3a81-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3a81-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b3a81-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b3a81-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3a81-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3a81-115">Not supported.</span></span>|
|<span data-ttu-id="b3a81-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b3a81-116">Application</span></span>|<span data-ttu-id="b3a81-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3a81-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3a81-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b3a81-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="b3a81-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3a81-119">Request headers</span></span>
|<span data-ttu-id="b3a81-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3a81-120">Header</span></span>|<span data-ttu-id="b3a81-121">値</span><span class="sxs-lookup"><span data-stu-id="b3a81-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3a81-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3a81-122">Authorization</span></span>|<span data-ttu-id="b3a81-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b3a81-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3a81-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b3a81-124">Accept</span></span>|<span data-ttu-id="b3a81-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b3a81-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3a81-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b3a81-126">Request body</span></span>
<span data-ttu-id="b3a81-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b3a81-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3a81-128">応答</span><span class="sxs-lookup"><span data-stu-id="b3a81-128">Response</span></span>
<span data-ttu-id="b3a81-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b3a81-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3a81-130">例</span><span class="sxs-lookup"><span data-stu-id="b3a81-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3a81-131">要求</span><span class="sxs-lookup"><span data-stu-id="b3a81-131">Request</span></span>
<span data-ttu-id="b3a81-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b3a81-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

### <a name="response"></a><span data-ttu-id="b3a81-133">応答</span><span class="sxs-lookup"><span data-stu-id="b3a81-133">Response</span></span>
<span data-ttu-id="b3a81-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b3a81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppDependency",
      "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
      "targetId": "Target Id value",
      "targetDisplayName": "Target Display Name value",
      "dependencyType": "autoInstall",
      "dependentAppCount": 1
    }
  ]
}
```





