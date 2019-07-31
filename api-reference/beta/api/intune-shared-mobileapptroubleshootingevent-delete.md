---
title: MobileAppTroubleshootingEvent の削除
description: 複数のワークフローをサポートする Microsoft Graph API for Intune の Delete mobileAppTroubleshootingEvent メソッドについて説明します。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b9ae2aafe9fe740d5156f2c756a03a9905aa995
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993586"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="71090-103">MobileAppTroubleshootingEvent の削除</span><span class="sxs-lookup"><span data-stu-id="71090-103">Delete mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="71090-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="71090-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="71090-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71090-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71090-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="71090-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71090-107">[MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="71090-107">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71090-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="71090-108">Prerequisites</span></span>
<span data-ttu-id="71090-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71090-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71090-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="71090-111">Permission type</span></span>|<span data-ttu-id="71090-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="71090-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71090-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="71090-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="71090-114">&nbsp;&nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="71090-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="71090-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71090-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="71090-116">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="71090-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="71090-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71090-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="71090-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="71090-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71090-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71090-119">Not supported.</span></span>|
|<span data-ttu-id="71090-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="71090-120">Application</span></span>|<span data-ttu-id="71090-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71090-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71090-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="71090-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="71090-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71090-123">Request headers</span></span>
|<span data-ttu-id="71090-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71090-124">Header</span></span>|<span data-ttu-id="71090-125">値</span><span class="sxs-lookup"><span data-stu-id="71090-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71090-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="71090-126">Authorization</span></span>|<span data-ttu-id="71090-127">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="71090-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71090-128">承諾</span><span class="sxs-lookup"><span data-stu-id="71090-128">Accept</span></span>|<span data-ttu-id="71090-129">application/json</span><span class="sxs-lookup"><span data-stu-id="71090-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71090-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="71090-130">Request body</span></span>
<span data-ttu-id="71090-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="71090-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71090-132">応答</span><span class="sxs-lookup"><span data-stu-id="71090-132">Response</span></span>
<span data-ttu-id="71090-133">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="71090-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="71090-134">例</span><span class="sxs-lookup"><span data-stu-id="71090-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="71090-135">要求</span><span class="sxs-lookup"><span data-stu-id="71090-135">Request</span></span>
<span data-ttu-id="71090-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="71090-136">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="71090-137">応答</span><span class="sxs-lookup"><span data-stu-id="71090-137">Response</span></span>
<span data-ttu-id="71090-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="71090-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




