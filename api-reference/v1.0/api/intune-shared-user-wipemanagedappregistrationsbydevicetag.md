---
title: wipeManagedAppRegistrationsByDeviceTag アクション
description: 指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bea86526d1c8770ac1800442d5e0f2e06318fb58
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025723"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="6433c-103">wipeManagedAppRegistrationsByDeviceTag アクション</span><span class="sxs-lookup"><span data-stu-id="6433c-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="6433c-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6433c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6433c-105">指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="6433c-105">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6433c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6433c-106">Prerequisites</span></span>
<span data-ttu-id="6433c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6433c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6433c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6433c-109">Permission type</span></span>|<span data-ttu-id="6433c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6433c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6433c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6433c-111">Delegated (work or school account)</span></span>| <span data-ttu-id="6433c-112">_コンテキストによって異なる_</span><span class="sxs-lookup"><span data-stu-id="6433c-112">_varies by context_</span></span> |
| <span data-ttu-id="6433c-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="6433c-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="6433c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6433c-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="6433c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6433c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6433c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6433c-116">Not supported.</span></span>|
|<span data-ttu-id="6433c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6433c-117">Application</span></span>|<span data-ttu-id="6433c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6433c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6433c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6433c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="6433c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6433c-120">Request headers</span></span>
|<span data-ttu-id="6433c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6433c-121">Header</span></span>|<span data-ttu-id="6433c-122">値</span><span class="sxs-lookup"><span data-stu-id="6433c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6433c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6433c-123">Authorization</span></span>|<span data-ttu-id="6433c-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6433c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6433c-125">承諾</span><span class="sxs-lookup"><span data-stu-id="6433c-125">Accept</span></span>|<span data-ttu-id="6433c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6433c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6433c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6433c-127">Request body</span></span>
<span data-ttu-id="6433c-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6433c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6433c-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="6433c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6433c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6433c-130">Property</span></span>|<span data-ttu-id="6433c-131">型</span><span class="sxs-lookup"><span data-stu-id="6433c-131">Type</span></span>|<span data-ttu-id="6433c-132">説明</span><span class="sxs-lookup"><span data-stu-id="6433c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6433c-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="6433c-133">deviceTag</span></span>|<span data-ttu-id="6433c-134">String</span><span class="sxs-lookup"><span data-stu-id="6433c-134">String</span></span>|<span data-ttu-id="6433c-135">デバイス タグ</span><span class="sxs-lookup"><span data-stu-id="6433c-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="6433c-136">応答</span><span class="sxs-lookup"><span data-stu-id="6433c-136">Response</span></span>
<span data-ttu-id="6433c-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="6433c-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6433c-138">例</span><span class="sxs-lookup"><span data-stu-id="6433c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="6433c-139">要求</span><span class="sxs-lookup"><span data-stu-id="6433c-139">Request</span></span>
<span data-ttu-id="6433c-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6433c-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="6433c-141">応答</span><span class="sxs-lookup"><span data-stu-id="6433c-141">Response</span></span>
<span data-ttu-id="6433c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6433c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



