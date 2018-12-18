---
title: wipeManagedAppRegistrationsByDeviceTag アクション
description: 指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。
author: tfitzmac
ms.openlocfilehash: c08ba0bb670b2429cd97f7a23a8790ccc6c5c487
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318971"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="8a45a-103">wipeManagedAppRegistrationsByDeviceTag アクション</span><span class="sxs-lookup"><span data-stu-id="8a45a-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="8a45a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8a45a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a45a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a45a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a45a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a45a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a45a-107">指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="8a45a-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a45a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8a45a-108">Prerequisites</span></span>

<span data-ttu-id="8a45a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a45a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a45a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a45a-111">Permission type</span></span>|<span data-ttu-id="8a45a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a45a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a45a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a45a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8a45a-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="8a45a-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="8a45a-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a45a-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8a45a-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a45a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a45a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a45a-117">Not supported.</span></span>|
|<span data-ttu-id="8a45a-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a45a-118">Application</span></span>|<span data-ttu-id="8a45a-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a45a-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a45a-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a45a-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="8a45a-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a45a-121">Request headers</span></span>

|<span data-ttu-id="8a45a-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a45a-122">Header</span></span>|<span data-ttu-id="8a45a-123">値</span><span class="sxs-lookup"><span data-stu-id="8a45a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a45a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a45a-124">Authorization</span></span>|<span data-ttu-id="8a45a-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8a45a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a45a-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8a45a-126">Accept</span></span>|<span data-ttu-id="8a45a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8a45a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a45a-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a45a-128">Request body</span></span>

<span data-ttu-id="8a45a-129">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8a45a-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8a45a-130">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="8a45a-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8a45a-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a45a-131">Property</span></span>|<span data-ttu-id="8a45a-132">種類</span><span class="sxs-lookup"><span data-stu-id="8a45a-132">Type</span></span>|<span data-ttu-id="8a45a-133">説明</span><span class="sxs-lookup"><span data-stu-id="8a45a-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a45a-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="8a45a-134">deviceTag</span></span>|<span data-ttu-id="8a45a-135">String</span><span class="sxs-lookup"><span data-stu-id="8a45a-135">String</span></span>|<span data-ttu-id="8a45a-136">デバイス タグ</span><span class="sxs-lookup"><span data-stu-id="8a45a-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="8a45a-137">応答</span><span class="sxs-lookup"><span data-stu-id="8a45a-137">Response</span></span>

<span data-ttu-id="8a45a-138">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="8a45a-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8a45a-139">例</span><span class="sxs-lookup"><span data-stu-id="8a45a-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a45a-140">要求</span><span class="sxs-lookup"><span data-stu-id="8a45a-140">Request</span></span>

<span data-ttu-id="8a45a-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8a45a-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="8a45a-142">応答</span><span class="sxs-lookup"><span data-stu-id="8a45a-142">Response</span></span>

<span data-ttu-id="8a45a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8a45a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






