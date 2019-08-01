---
title: Delete iosCustomConfiguration
description: iosCustomConfiguration を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3faea675124325b6f7da0ae0c5eeb8fa37a34661
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018954"
---
# <a name="delete-ioscustomconfiguration"></a><span data-ttu-id="1cf8f-103">Delete iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="1cf8f-103">Delete iosCustomConfiguration</span></span>

> <span data-ttu-id="1cf8f-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1cf8f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cf8f-105">[iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="1cf8f-105">Deletes a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1cf8f-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1cf8f-106">Prerequisites</span></span>
<span data-ttu-id="1cf8f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1cf8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cf8f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1cf8f-109">Permission type</span></span>|<span data-ttu-id="1cf8f-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1cf8f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cf8f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1cf8f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1cf8f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cf8f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1cf8f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1cf8f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cf8f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1cf8f-114">Not supported.</span></span>|
|<span data-ttu-id="1cf8f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1cf8f-115">Application</span></span>|<span data-ttu-id="1cf8f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1cf8f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cf8f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1cf8f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1cf8f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1cf8f-118">Request headers</span></span>
|<span data-ttu-id="1cf8f-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1cf8f-119">Header</span></span>|<span data-ttu-id="1cf8f-120">値</span><span class="sxs-lookup"><span data-stu-id="1cf8f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cf8f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cf8f-121">Authorization</span></span>|<span data-ttu-id="1cf8f-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1cf8f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cf8f-123">承諾</span><span class="sxs-lookup"><span data-stu-id="1cf8f-123">Accept</span></span>|<span data-ttu-id="1cf8f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1cf8f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cf8f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1cf8f-125">Request body</span></span>
<span data-ttu-id="1cf8f-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1cf8f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cf8f-127">応答</span><span class="sxs-lookup"><span data-stu-id="1cf8f-127">Response</span></span>
<span data-ttu-id="1cf8f-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="1cf8f-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1cf8f-129">例</span><span class="sxs-lookup"><span data-stu-id="1cf8f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="1cf8f-130">要求</span><span class="sxs-lookup"><span data-stu-id="1cf8f-130">Request</span></span>
<span data-ttu-id="1cf8f-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1cf8f-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="1cf8f-132">応答</span><span class="sxs-lookup"><span data-stu-id="1cf8f-132">Response</span></span>
<span data-ttu-id="1cf8f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1cf8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



