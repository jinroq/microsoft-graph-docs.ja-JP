---
title: wipeManagedAppRegistrationsByDeviceTag アクション
description: 指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b4d74df507e3172713fea4179b321fdf05cc06be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576662"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="dc911-103">wipeManagedAppRegistrationsByDeviceTag アクション</span><span class="sxs-lookup"><span data-stu-id="dc911-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="dc911-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dc911-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc911-105">指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="dc911-105">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc911-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="dc911-106">Prerequisites</span></span>
<span data-ttu-id="dc911-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc911-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc911-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dc911-109">Permission type</span></span>|<span data-ttu-id="dc911-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dc911-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc911-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dc911-111">Delegated (work or school account)</span></span>| <span data-ttu-id="dc911-112">_コンテキストによって異なる_</span><span class="sxs-lookup"><span data-stu-id="dc911-112">_varies by context_</span></span> |
| <span data-ttu-id="dc911-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="dc911-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="dc911-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc911-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="dc911-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dc911-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc911-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc911-116">Not supported.</span></span>|
|<span data-ttu-id="dc911-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dc911-117">Application</span></span>|<span data-ttu-id="dc911-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc911-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc911-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dc911-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="dc911-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc911-120">Request headers</span></span>
|<span data-ttu-id="dc911-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc911-121">Header</span></span>|<span data-ttu-id="dc911-122">値</span><span class="sxs-lookup"><span data-stu-id="dc911-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc911-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc911-123">Authorization</span></span>|<span data-ttu-id="dc911-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="dc911-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc911-125">承諾</span><span class="sxs-lookup"><span data-stu-id="dc911-125">Accept</span></span>|<span data-ttu-id="dc911-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc911-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc911-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="dc911-127">Request body</span></span>
<span data-ttu-id="dc911-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dc911-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dc911-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="dc911-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dc911-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc911-130">Property</span></span>|<span data-ttu-id="dc911-131">型</span><span class="sxs-lookup"><span data-stu-id="dc911-131">Type</span></span>|<span data-ttu-id="dc911-132">説明</span><span class="sxs-lookup"><span data-stu-id="dc911-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc911-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="dc911-133">deviceTag</span></span>|<span data-ttu-id="dc911-134">String</span><span class="sxs-lookup"><span data-stu-id="dc911-134">String</span></span>|<span data-ttu-id="dc911-135">デバイス タグ</span><span class="sxs-lookup"><span data-stu-id="dc911-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="dc911-136">応答</span><span class="sxs-lookup"><span data-stu-id="dc911-136">Response</span></span>
<span data-ttu-id="dc911-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="dc911-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dc911-138">例</span><span class="sxs-lookup"><span data-stu-id="dc911-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc911-139">要求</span><span class="sxs-lookup"><span data-stu-id="dc911-139">Request</span></span>
<span data-ttu-id="dc911-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dc911-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="dc911-141">応答</span><span class="sxs-lookup"><span data-stu-id="dc911-141">Response</span></span>
<span data-ttu-id="dc911-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dc911-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



