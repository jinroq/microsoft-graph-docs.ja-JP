---
title: リスト mobileAppTroubleshootingEvents
description: Intune は、複数のワークフローをサポートする Microsoft のグラフの API のリスト mobileAppTroubleshootingEvent のメソッドについて説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 79f89fd755b52bc0d9a3a1a1d0e0c6dc91853e76
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430410"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="9b34f-103">リスト mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="9b34f-103">List mobileAppTroubleshootingEvents</span></span>

> <span data-ttu-id="9b34f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9b34f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9b34f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b34f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b34f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9b34f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b34f-107">[MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9b34f-107">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b34f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9b34f-108">Prerequisites</span></span>
<span data-ttu-id="9b34f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b34f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9b34f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9b34f-111">Permission type</span></span>|<span data-ttu-id="9b34f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9b34f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b34f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9b34f-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="9b34f-114">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="9b34f-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="9b34f-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b34f-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9b34f-116">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="9b34f-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="9b34f-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b34f-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9b34f-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b34f-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b34f-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b34f-119">Not supported.</span></span>|
|<span data-ttu-id="9b34f-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b34f-120">Application</span></span>|<span data-ttu-id="9b34f-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b34f-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b34f-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9b34f-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="9b34f-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b34f-123">Request headers</span></span>
|<span data-ttu-id="9b34f-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b34f-124">Header</span></span>|<span data-ttu-id="9b34f-125">値</span><span class="sxs-lookup"><span data-stu-id="9b34f-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b34f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b34f-126">Authorization</span></span>|<span data-ttu-id="9b34f-127">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9b34f-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b34f-128">Accept</span><span class="sxs-lookup"><span data-stu-id="9b34f-128">Accept</span></span>|<span data-ttu-id="9b34f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="9b34f-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b34f-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="9b34f-130">Request body</span></span>
<span data-ttu-id="9b34f-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9b34f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b34f-132">応答</span><span class="sxs-lookup"><span data-stu-id="9b34f-132">Response</span></span>
<span data-ttu-id="9b34f-133">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="9b34f-133">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b34f-134">例</span><span class="sxs-lookup"><span data-stu-id="9b34f-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b34f-135">要求</span><span class="sxs-lookup"><span data-stu-id="9b34f-135">Request</span></span>
<span data-ttu-id="9b34f-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9b34f-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="9b34f-137">応答</span><span class="sxs-lookup"><span data-stu-id="9b34f-137">Response</span></span>
<span data-ttu-id="9b34f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9b34f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
      "id": "77943c10-3c10-7794-103c-9477103c9477"
    }
  ]
}
```




