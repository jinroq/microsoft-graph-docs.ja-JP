---
title: mobileAppTroubleshootingEvent を取得する
description: 複数のワークフローをサポートする Microsoft Graph API for Intune の Get mobileAppTroubleshootingEvent メソッドについて説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 474108fc1e6345a9fb436acf877a2aa1daf9c401
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526966"
---
# <a name="get-mobileapptroubleshootingevent"></a><span data-ttu-id="2bc64-103">mobileAppTroubleshootingEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="2bc64-103">Get mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="2bc64-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="2bc64-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2bc64-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2bc64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2bc64-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2bc64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bc64-107">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2bc64-107">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bc64-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2bc64-108">Prerequisites</span></span>
<span data-ttu-id="2bc64-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2bc64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bc64-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2bc64-111">Permission type</span></span>|<span data-ttu-id="2bc64-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2bc64-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bc64-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2bc64-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="2bc64-114">&nbsp;&nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="2bc64-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="2bc64-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bc64-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="2bc64-116">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="2bc64-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="2bc64-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bc64-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="2bc64-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2bc64-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bc64-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2bc64-119">Not supported.</span></span>|
|<span data-ttu-id="2bc64-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2bc64-120">Application</span></span>|<span data-ttu-id="2bc64-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2bc64-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bc64-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2bc64-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
GET /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2bc64-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2bc64-123">Optional query parameters</span></span>
<span data-ttu-id="2bc64-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2bc64-124">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2bc64-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2bc64-125">Request headers</span></span>
|<span data-ttu-id="2bc64-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2bc64-126">Header</span></span>|<span data-ttu-id="2bc64-127">値</span><span class="sxs-lookup"><span data-stu-id="2bc64-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bc64-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bc64-128">Authorization</span></span>|<span data-ttu-id="2bc64-129">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2bc64-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bc64-130">承諾</span><span class="sxs-lookup"><span data-stu-id="2bc64-130">Accept</span></span>|<span data-ttu-id="2bc64-131">application/json</span><span class="sxs-lookup"><span data-stu-id="2bc64-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bc64-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="2bc64-132">Request body</span></span>
<span data-ttu-id="2bc64-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2bc64-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bc64-134">応答</span><span class="sxs-lookup"><span data-stu-id="2bc64-134">Response</span></span>
<span data-ttu-id="2bc64-135">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2bc64-135">If successful, this method returns a `200 OK` response code and [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bc64-136">例</span><span class="sxs-lookup"><span data-stu-id="2bc64-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bc64-137">要求</span><span class="sxs-lookup"><span data-stu-id="2bc64-137">Request</span></span>
<span data-ttu-id="2bc64-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2bc64-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="2bc64-139">応答</span><span class="sxs-lookup"><span data-stu-id="2bc64-139">Response</span></span>
<span data-ttu-id="2bc64-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2bc64-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 143

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
    "id": "77943c10-3c10-7794-103c-9477103c9477"
  }
}
```




