---
title: sync アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 98e2c1671b7fde9450b18ca3bd12537450d02416
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988477"
---
# <a name="sync-action"></a><span data-ttu-id="91991-103">同期アクション</span><span class="sxs-lookup"><span data-stu-id="91991-103">sync action</span></span>

> <span data-ttu-id="91991-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="91991-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91991-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="91991-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91991-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="91991-106">Prerequisites</span></span>
<span data-ttu-id="91991-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91991-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91991-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="91991-109">Permission type</span></span>|<span data-ttu-id="91991-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="91991-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91991-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="91991-111">Delegated (work or school account)</span></span>|<span data-ttu-id="91991-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91991-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="91991-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="91991-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91991-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91991-114">Not supported.</span></span>|
|<span data-ttu-id="91991-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="91991-115">Application</span></span>|<span data-ttu-id="91991-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91991-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91991-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="91991-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="91991-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91991-118">Request headers</span></span>
|<span data-ttu-id="91991-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91991-119">Header</span></span>|<span data-ttu-id="91991-120">値</span><span class="sxs-lookup"><span data-stu-id="91991-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91991-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="91991-121">Authorization</span></span>|<span data-ttu-id="91991-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="91991-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91991-123">承諾</span><span class="sxs-lookup"><span data-stu-id="91991-123">Accept</span></span>|<span data-ttu-id="91991-124">application/json</span><span class="sxs-lookup"><span data-stu-id="91991-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91991-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="91991-125">Request body</span></span>
<span data-ttu-id="91991-126">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="91991-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="91991-127">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="91991-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="91991-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91991-128">Property</span></span>|<span data-ttu-id="91991-129">型</span><span class="sxs-lookup"><span data-stu-id="91991-129">Type</span></span>|<span data-ttu-id="91991-130">説明</span><span class="sxs-lookup"><span data-stu-id="91991-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91991-131">syncType</span><span class="sxs-lookup"><span data-stu-id="91991-131">syncType</span></span>|[<span data-ttu-id="91991-132">deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="91991-132">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="91991-133">実行される同期の種類。完全同期またはデルタ同期のどちらかです。</span><span class="sxs-lookup"><span data-stu-id="91991-133">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="91991-134">応答</span><span class="sxs-lookup"><span data-stu-id="91991-134">Response</span></span>
<span data-ttu-id="91991-135">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="91991-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="91991-136">例</span><span class="sxs-lookup"><span data-stu-id="91991-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="91991-137">要求</span><span class="sxs-lookup"><span data-stu-id="91991-137">Request</span></span>
<span data-ttu-id="91991-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="91991-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="91991-139">応答</span><span class="sxs-lookup"><span data-stu-id="91991-139">Response</span></span>
<span data-ttu-id="91991-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="91991-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



