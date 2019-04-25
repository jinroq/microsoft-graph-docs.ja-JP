---
title: revokeLicenses アクション
description: 特定の appleVolumePurchaseProgramToken に関連付けられているライセンスを取り消す
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d6799edd63f555275ea5f4142844c55611923ac5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527932"
---
# <a name="revokelicenses-action"></a><span data-ttu-id="f194a-103">revokeLicenses アクション</span><span class="sxs-lookup"><span data-stu-id="f194a-103">revokeLicenses action</span></span>

> <span data-ttu-id="f194a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f194a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f194a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f194a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f194a-106">特定の appleVolumePurchaseProgramToken に関連付けられているライセンスを取り消す</span><span class="sxs-lookup"><span data-stu-id="f194a-106">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f194a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f194a-107">Prerequisites</span></span>
<span data-ttu-id="f194a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f194a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f194a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f194a-110">Permission type</span></span>|<span data-ttu-id="f194a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f194a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f194a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f194a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f194a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f194a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f194a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f194a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f194a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f194a-115">Not supported.</span></span>|
|<span data-ttu-id="f194a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f194a-116">Application</span></span>|<span data-ttu-id="f194a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f194a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f194a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f194a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses
```

## <a name="request-headers"></a><span data-ttu-id="f194a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f194a-119">Request headers</span></span>
|<span data-ttu-id="f194a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f194a-120">Header</span></span>|<span data-ttu-id="f194a-121">値</span><span class="sxs-lookup"><span data-stu-id="f194a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f194a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f194a-122">Authorization</span></span>|<span data-ttu-id="f194a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f194a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f194a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f194a-124">Accept</span></span>|<span data-ttu-id="f194a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f194a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f194a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f194a-126">Request body</span></span>
<span data-ttu-id="f194a-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f194a-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f194a-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="f194a-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f194a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f194a-129">Property</span></span>|<span data-ttu-id="f194a-130">型</span><span class="sxs-lookup"><span data-stu-id="f194a-130">Type</span></span>|<span data-ttu-id="f194a-131">説明</span><span class="sxs-lookup"><span data-stu-id="f194a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f194a-132">notifymanageddevices</span><span class="sxs-lookup"><span data-stu-id="f194a-132">notifyManagedDevices</span></span>|<span data-ttu-id="f194a-133">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="f194a-133">Boolean</span></span>|<span data-ttu-id="f194a-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f194a-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f194a-135">応答</span><span class="sxs-lookup"><span data-stu-id="f194a-135">Response</span></span>
<span data-ttu-id="f194a-136">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f194a-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f194a-137">例</span><span class="sxs-lookup"><span data-stu-id="f194a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f194a-138">要求</span><span class="sxs-lookup"><span data-stu-id="f194a-138">Request</span></span>
<span data-ttu-id="f194a-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f194a-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="f194a-140">応答</span><span class="sxs-lookup"><span data-stu-id="f194a-140">Response</span></span>
<span data-ttu-id="f194a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f194a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





