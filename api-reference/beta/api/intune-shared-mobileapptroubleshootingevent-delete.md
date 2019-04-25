---
title: mobileAppTroubleshootingEvent の削除
description: 複数のワークフローをサポートする Microsoft Graph API for Intune の Delete mobileAppTroubleshootingEvent メソッドについて説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 41c9383524e29ff897ea255555ab663476c36659
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527148"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="2afdc-103">mobileAppTroubleshootingEvent の削除</span><span class="sxs-lookup"><span data-stu-id="2afdc-103">Delete mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="2afdc-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="2afdc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2afdc-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2afdc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2afdc-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2afdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2afdc-107">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="2afdc-107">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2afdc-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2afdc-108">Prerequisites</span></span>
<span data-ttu-id="2afdc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2afdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2afdc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2afdc-111">Permission type</span></span>|<span data-ttu-id="2afdc-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2afdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2afdc-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2afdc-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="2afdc-114">&nbsp;&nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="2afdc-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="2afdc-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2afdc-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2afdc-116">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="2afdc-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="2afdc-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2afdc-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2afdc-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2afdc-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2afdc-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2afdc-119">Not supported.</span></span>|
|<span data-ttu-id="2afdc-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2afdc-120">Application</span></span>|<span data-ttu-id="2afdc-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2afdc-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2afdc-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2afdc-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="2afdc-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2afdc-123">Request headers</span></span>
|<span data-ttu-id="2afdc-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2afdc-124">Header</span></span>|<span data-ttu-id="2afdc-125">値</span><span class="sxs-lookup"><span data-stu-id="2afdc-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2afdc-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2afdc-126">Authorization</span></span>|<span data-ttu-id="2afdc-127">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2afdc-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2afdc-128">承諾</span><span class="sxs-lookup"><span data-stu-id="2afdc-128">Accept</span></span>|<span data-ttu-id="2afdc-129">application/json</span><span class="sxs-lookup"><span data-stu-id="2afdc-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2afdc-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="2afdc-130">Request body</span></span>
<span data-ttu-id="2afdc-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2afdc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2afdc-132">応答</span><span class="sxs-lookup"><span data-stu-id="2afdc-132">Response</span></span>
<span data-ttu-id="2afdc-133">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="2afdc-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2afdc-134">例</span><span class="sxs-lookup"><span data-stu-id="2afdc-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="2afdc-135">要求</span><span class="sxs-lookup"><span data-stu-id="2afdc-135">Request</span></span>
<span data-ttu-id="2afdc-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2afdc-136">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="2afdc-137">応答</span><span class="sxs-lookup"><span data-stu-id="2afdc-137">Response</span></span>
<span data-ttu-id="2afdc-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2afdc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




