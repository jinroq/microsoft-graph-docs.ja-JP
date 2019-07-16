---
title: wipeManagedAppRegistrationByDeviceTag アクション
description: 指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe1c455791414757127aa90b27cc9ec494ed2f86
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726102"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a><span data-ttu-id="3148d-103">wipeManagedAppRegistrationByDeviceTag アクション</span><span class="sxs-lookup"><span data-stu-id="3148d-103">wipeManagedAppRegistrationByDeviceTag action</span></span>

> <span data-ttu-id="3148d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3148d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3148d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3148d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3148d-106">指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="3148d-106">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3148d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3148d-107">Prerequisites</span></span>
<span data-ttu-id="3148d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3148d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3148d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3148d-110">Permission type</span></span>|<span data-ttu-id="3148d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3148d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3148d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3148d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3148d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3148d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3148d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3148d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3148d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3148d-115">Not supported.</span></span>|
|<span data-ttu-id="3148d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3148d-116">Application</span></span>|<span data-ttu-id="3148d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3148d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3148d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3148d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="3148d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3148d-119">Request headers</span></span>
|<span data-ttu-id="3148d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3148d-120">Header</span></span>|<span data-ttu-id="3148d-121">値</span><span class="sxs-lookup"><span data-stu-id="3148d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3148d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3148d-122">Authorization</span></span>|<span data-ttu-id="3148d-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3148d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3148d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3148d-124">Accept</span></span>|<span data-ttu-id="3148d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3148d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3148d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3148d-126">Request body</span></span>
<span data-ttu-id="3148d-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3148d-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3148d-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="3148d-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3148d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3148d-129">Property</span></span>|<span data-ttu-id="3148d-130">型</span><span class="sxs-lookup"><span data-stu-id="3148d-130">Type</span></span>|<span data-ttu-id="3148d-131">説明</span><span class="sxs-lookup"><span data-stu-id="3148d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3148d-132">deviceTag</span><span class="sxs-lookup"><span data-stu-id="3148d-132">deviceTag</span></span>|<span data-ttu-id="3148d-133">String</span><span class="sxs-lookup"><span data-stu-id="3148d-133">String</span></span>|<span data-ttu-id="3148d-134">デバイス タグ</span><span class="sxs-lookup"><span data-stu-id="3148d-134">device tag</span></span>|



## <a name="response"></a><span data-ttu-id="3148d-135">応答</span><span class="sxs-lookup"><span data-stu-id="3148d-135">Response</span></span>
<span data-ttu-id="3148d-136">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="3148d-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3148d-137">例</span><span class="sxs-lookup"><span data-stu-id="3148d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="3148d-138">要求</span><span class="sxs-lookup"><span data-stu-id="3148d-138">Request</span></span>
<span data-ttu-id="3148d-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3148d-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="3148d-140">応答</span><span class="sxs-lookup"><span data-stu-id="3148d-140">Response</span></span>
<span data-ttu-id="3148d-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3148d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





