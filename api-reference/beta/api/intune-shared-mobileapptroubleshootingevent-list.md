---
title: リスト mobileAppTroubleshootingEvents
description: 複数のワークフローをサポートする Microsoft Graph API for Intune の List mobileAppTroubleshootingEvent メソッドについて説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d34d37324e61e967b01b46e2a1ba842688862281
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976870"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="c370f-103">リスト mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="c370f-103">List mobileAppTroubleshootingEvents</span></span>

> <span data-ttu-id="c370f-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="c370f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c370f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c370f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c370f-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c370f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c370f-107">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c370f-107">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c370f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c370f-108">Prerequisites</span></span>
<span data-ttu-id="c370f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c370f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c370f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c370f-111">Permission type</span></span>|<span data-ttu-id="c370f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c370f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c370f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c370f-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="c370f-114">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="c370f-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="c370f-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c370f-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c370f-116">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="c370f-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="c370f-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c370f-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c370f-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c370f-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c370f-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c370f-119">Not supported.</span></span>|
|<span data-ttu-id="c370f-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c370f-120">Application</span></span>|<span data-ttu-id="c370f-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c370f-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c370f-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c370f-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="c370f-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c370f-123">Request headers</span></span>
|<span data-ttu-id="c370f-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c370f-124">Header</span></span>|<span data-ttu-id="c370f-125">値</span><span class="sxs-lookup"><span data-stu-id="c370f-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c370f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c370f-126">Authorization</span></span>|<span data-ttu-id="c370f-127">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c370f-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c370f-128">承諾</span><span class="sxs-lookup"><span data-stu-id="c370f-128">Accept</span></span>|<span data-ttu-id="c370f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="c370f-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c370f-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="c370f-130">Request body</span></span>
<span data-ttu-id="c370f-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c370f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c370f-132">応答</span><span class="sxs-lookup"><span data-stu-id="c370f-132">Response</span></span>
<span data-ttu-id="c370f-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c370f-133">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c370f-134">例</span><span class="sxs-lookup"><span data-stu-id="c370f-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="c370f-135">要求</span><span class="sxs-lookup"><span data-stu-id="c370f-135">Request</span></span>
<span data-ttu-id="c370f-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c370f-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="c370f-137">応答</span><span class="sxs-lookup"><span data-stu-id="c370f-137">Response</span></span>
<span data-ttu-id="c370f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c370f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




