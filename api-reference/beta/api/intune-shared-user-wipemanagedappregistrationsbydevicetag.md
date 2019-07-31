---
title: wipeManagedAppRegistrationsByDeviceTag アクション
description: 指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bf4c11edbd0743c3ef4e641496cfb851e347b995
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984084"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="1824d-103">wipeManagedAppRegistrationsByDeviceTag アクション</span><span class="sxs-lookup"><span data-stu-id="1824d-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="1824d-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1824d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1824d-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1824d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1824d-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1824d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1824d-107">指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="1824d-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1824d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1824d-108">Prerequisites</span></span>

<span data-ttu-id="1824d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1824d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1824d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1824d-111">Permission type</span></span>|<span data-ttu-id="1824d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1824d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1824d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1824d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1824d-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="1824d-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="1824d-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1824d-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1824d-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1824d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1824d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1824d-117">Not supported.</span></span>|
|<span data-ttu-id="1824d-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1824d-118">Application</span></span>|<span data-ttu-id="1824d-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1824d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1824d-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1824d-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="1824d-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1824d-121">Request headers</span></span>

|<span data-ttu-id="1824d-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1824d-122">Header</span></span>|<span data-ttu-id="1824d-123">値</span><span class="sxs-lookup"><span data-stu-id="1824d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1824d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1824d-124">Authorization</span></span>|<span data-ttu-id="1824d-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1824d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1824d-126">承諾</span><span class="sxs-lookup"><span data-stu-id="1824d-126">Accept</span></span>|<span data-ttu-id="1824d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1824d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1824d-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="1824d-128">Request body</span></span>

<span data-ttu-id="1824d-129">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1824d-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1824d-130">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="1824d-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1824d-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1824d-131">Property</span></span>|<span data-ttu-id="1824d-132">型</span><span class="sxs-lookup"><span data-stu-id="1824d-132">Type</span></span>|<span data-ttu-id="1824d-133">説明</span><span class="sxs-lookup"><span data-stu-id="1824d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1824d-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="1824d-134">deviceTag</span></span>|<span data-ttu-id="1824d-135">String</span><span class="sxs-lookup"><span data-stu-id="1824d-135">String</span></span>|<span data-ttu-id="1824d-136">デバイス タグ</span><span class="sxs-lookup"><span data-stu-id="1824d-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="1824d-137">応答</span><span class="sxs-lookup"><span data-stu-id="1824d-137">Response</span></span>

<span data-ttu-id="1824d-138">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="1824d-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1824d-139">例</span><span class="sxs-lookup"><span data-stu-id="1824d-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="1824d-140">要求</span><span class="sxs-lookup"><span data-stu-id="1824d-140">Request</span></span>

<span data-ttu-id="1824d-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1824d-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="1824d-142">応答</span><span class="sxs-lookup"><span data-stu-id="1824d-142">Response</span></span>

<span data-ttu-id="1824d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1824d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






