---
title: wipeManagedAppRegistrationsByDeviceTag アクション
description: 指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 08002aefd92bda80c8c5a47e261201434777cea4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962128"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="f09a9-103">wipeManagedAppRegistrationsByDeviceTag アクション</span><span class="sxs-lookup"><span data-stu-id="f09a9-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="f09a9-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f09a9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f09a9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f09a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f09a9-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f09a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f09a9-107">指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="f09a9-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f09a9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f09a9-108">Prerequisites</span></span>

<span data-ttu-id="f09a9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f09a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f09a9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f09a9-111">Permission type</span></span>|<span data-ttu-id="f09a9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f09a9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f09a9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f09a9-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f09a9-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="f09a9-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="f09a9-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f09a9-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f09a9-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f09a9-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f09a9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f09a9-117">Not supported.</span></span>|
|<span data-ttu-id="f09a9-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f09a9-118">Application</span></span>|<span data-ttu-id="f09a9-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f09a9-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f09a9-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f09a9-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="f09a9-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f09a9-121">Request headers</span></span>

|<span data-ttu-id="f09a9-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f09a9-122">Header</span></span>|<span data-ttu-id="f09a9-123">値</span><span class="sxs-lookup"><span data-stu-id="f09a9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f09a9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f09a9-124">Authorization</span></span>|<span data-ttu-id="f09a9-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f09a9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f09a9-126">承諾</span><span class="sxs-lookup"><span data-stu-id="f09a9-126">Accept</span></span>|<span data-ttu-id="f09a9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f09a9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f09a9-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f09a9-128">Request body</span></span>

<span data-ttu-id="f09a9-129">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f09a9-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f09a9-130">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="f09a9-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f09a9-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f09a9-131">Property</span></span>|<span data-ttu-id="f09a9-132">型</span><span class="sxs-lookup"><span data-stu-id="f09a9-132">Type</span></span>|<span data-ttu-id="f09a9-133">説明</span><span class="sxs-lookup"><span data-stu-id="f09a9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f09a9-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="f09a9-134">deviceTag</span></span>|<span data-ttu-id="f09a9-135">String</span><span class="sxs-lookup"><span data-stu-id="f09a9-135">String</span></span>|<span data-ttu-id="f09a9-136">デバイス タグ</span><span class="sxs-lookup"><span data-stu-id="f09a9-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="f09a9-137">応答</span><span class="sxs-lookup"><span data-stu-id="f09a9-137">Response</span></span>

<span data-ttu-id="f09a9-138">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f09a9-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f09a9-139">例</span><span class="sxs-lookup"><span data-stu-id="f09a9-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="f09a9-140">要求</span><span class="sxs-lookup"><span data-stu-id="f09a9-140">Request</span></span>

<span data-ttu-id="f09a9-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f09a9-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="f09a9-142">応答</span><span class="sxs-lookup"><span data-stu-id="f09a9-142">Response</span></span>

<span data-ttu-id="f09a9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f09a9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






