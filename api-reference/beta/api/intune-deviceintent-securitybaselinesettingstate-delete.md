---
title: securityBaselineSettingState の削除
description: securityBaselineSettingState を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f69ac521929963cc0482bfb7e752b72670636d6
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522812"
---
# <a name="delete-securitybaselinesettingstate"></a><span data-ttu-id="320f0-103">securityBaselineSettingState の削除</span><span class="sxs-lookup"><span data-stu-id="320f0-103">Delete securityBaselineSettingState</span></span>

> <span data-ttu-id="320f0-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="320f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="320f0-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="320f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="320f0-106">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="320f0-106">Deletes a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="320f0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="320f0-107">Prerequisites</span></span>
<span data-ttu-id="320f0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="320f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="320f0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="320f0-110">Permission type</span></span>|<span data-ttu-id="320f0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="320f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="320f0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="320f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="320f0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="320f0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="320f0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="320f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="320f0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="320f0-115">Not supported.</span></span>|
|<span data-ttu-id="320f0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="320f0-116">Application</span></span>|<span data-ttu-id="320f0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="320f0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="320f0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="320f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="320f0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="320f0-119">Request headers</span></span>
|<span data-ttu-id="320f0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="320f0-120">Header</span></span>|<span data-ttu-id="320f0-121">値</span><span class="sxs-lookup"><span data-stu-id="320f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="320f0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="320f0-122">Authorization</span></span>|<span data-ttu-id="320f0-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="320f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="320f0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="320f0-124">Accept</span></span>|<span data-ttu-id="320f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="320f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="320f0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="320f0-126">Request body</span></span>
<span data-ttu-id="320f0-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="320f0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="320f0-128">応答</span><span class="sxs-lookup"><span data-stu-id="320f0-128">Response</span></span>
<span data-ttu-id="320f0-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="320f0-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="320f0-130">例</span><span class="sxs-lookup"><span data-stu-id="320f0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="320f0-131">要求</span><span class="sxs-lookup"><span data-stu-id="320f0-131">Request</span></span>
<span data-ttu-id="320f0-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="320f0-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
```

### <a name="response"></a><span data-ttu-id="320f0-133">応答</span><span class="sxs-lookup"><span data-stu-id="320f0-133">Response</span></span>
<span data-ttu-id="320f0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="320f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



