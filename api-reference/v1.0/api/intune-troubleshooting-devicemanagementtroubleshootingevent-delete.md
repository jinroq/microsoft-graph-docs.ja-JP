---
title: deviceManagementTroubleshootingEvent の削除
description: deviceManagementTroubleshootingEvent を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bbe75792e691cfd255af3ac82e2045d5a5e53724
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967329"
---
# <a name="delete-devicemanagementtroubleshootingevent"></a><span data-ttu-id="ff140-103">deviceManagementTroubleshootingEvent の削除</span><span class="sxs-lookup"><span data-stu-id="ff140-103">Delete deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="ff140-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ff140-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff140-105">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="ff140-105">Deletes a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff140-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="ff140-106">Prerequisites</span></span>
<span data-ttu-id="ff140-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff140-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff140-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff140-109">Permission type</span></span>|<span data-ttu-id="ff140-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff140-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff140-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff140-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ff140-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff140-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ff140-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff140-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff140-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff140-114">Not supported.</span></span>|
|<span data-ttu-id="ff140-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff140-115">Application</span></span>|<span data-ttu-id="ff140-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff140-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff140-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff140-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="ff140-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff140-118">Request headers</span></span>
|<span data-ttu-id="ff140-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff140-119">Header</span></span>|<span data-ttu-id="ff140-120">値</span><span class="sxs-lookup"><span data-stu-id="ff140-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff140-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff140-121">Authorization</span></span>|<span data-ttu-id="ff140-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ff140-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff140-123">承諾</span><span class="sxs-lookup"><span data-stu-id="ff140-123">Accept</span></span>|<span data-ttu-id="ff140-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ff140-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff140-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff140-125">Request body</span></span>
<span data-ttu-id="ff140-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ff140-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff140-127">応答</span><span class="sxs-lookup"><span data-stu-id="ff140-127">Response</span></span>
<span data-ttu-id="ff140-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ff140-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ff140-129">例</span><span class="sxs-lookup"><span data-stu-id="ff140-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff140-130">要求</span><span class="sxs-lookup"><span data-stu-id="ff140-130">Request</span></span>
<span data-ttu-id="ff140-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ff140-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="ff140-132">応答</span><span class="sxs-lookup"><span data-stu-id="ff140-132">Response</span></span>
<span data-ttu-id="ff140-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ff140-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



