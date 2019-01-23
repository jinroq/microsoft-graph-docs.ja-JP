---
title: MobileAppTroubleshootingEvent を削除します。
description: Intune は、複数のワークフローをサポートする Microsoft グラフ API の削除 mobileAppTroubleshootingEvent のメソッドについて説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fe83eccd4a4b289556234aef28be9e8764ad68ff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431632"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="43713-103">MobileAppTroubleshootingEvent を削除します。</span><span class="sxs-lookup"><span data-stu-id="43713-103">Delete mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="43713-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="43713-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="43713-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43713-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43713-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="43713-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43713-107">の[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="43713-107">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43713-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="43713-108">Prerequisites</span></span>
<span data-ttu-id="43713-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43713-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="43713-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="43713-111">Permission type</span></span>|<span data-ttu-id="43713-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="43713-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43713-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="43713-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="43713-114">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="43713-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="43713-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43713-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="43713-116">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="43713-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="43713-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43713-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="43713-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="43713-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43713-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43713-119">Not supported.</span></span>|
|<span data-ttu-id="43713-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="43713-120">Application</span></span>|<span data-ttu-id="43713-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43713-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43713-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="43713-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="43713-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43713-123">Request headers</span></span>
|<span data-ttu-id="43713-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43713-124">Header</span></span>|<span data-ttu-id="43713-125">値</span><span class="sxs-lookup"><span data-stu-id="43713-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43713-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="43713-126">Authorization</span></span>|<span data-ttu-id="43713-127">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="43713-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43713-128">Accept</span><span class="sxs-lookup"><span data-stu-id="43713-128">Accept</span></span>|<span data-ttu-id="43713-129">application/json</span><span class="sxs-lookup"><span data-stu-id="43713-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43713-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="43713-130">Request body</span></span>
<span data-ttu-id="43713-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="43713-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43713-132">応答</span><span class="sxs-lookup"><span data-stu-id="43713-132">Response</span></span>
<span data-ttu-id="43713-133">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="43713-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="43713-134">例</span><span class="sxs-lookup"><span data-stu-id="43713-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="43713-135">要求</span><span class="sxs-lookup"><span data-stu-id="43713-135">Request</span></span>
<span data-ttu-id="43713-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="43713-136">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="43713-137">応答</span><span class="sxs-lookup"><span data-stu-id="43713-137">Response</span></span>
<span data-ttu-id="43713-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="43713-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




