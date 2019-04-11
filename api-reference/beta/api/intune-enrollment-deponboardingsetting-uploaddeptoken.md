---
title: uploadDepToken アクション
description: 新しいデバイス登録プログラムトークンをアップロードする
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 553f0156304d69af79ca957a9d05a0115a41d93a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807883"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="f1c38-103">uploadDepToken アクション</span><span class="sxs-lookup"><span data-stu-id="f1c38-103">uploadDepToken action</span></span>

> <span data-ttu-id="f1c38-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1c38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1c38-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f1c38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1c38-106">新しいデバイス登録プログラムトークンをアップロードする</span><span class="sxs-lookup"><span data-stu-id="f1c38-106">Uploads a new Device Enrollment Program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1c38-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f1c38-107">Prerequisites</span></span>
<span data-ttu-id="f1c38-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1c38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1c38-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1c38-110">Permission type</span></span>|<span data-ttu-id="f1c38-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1c38-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1c38-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1c38-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1c38-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1c38-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f1c38-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1c38-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1c38-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1c38-115">Not supported.</span></span>|
|<span data-ttu-id="f1c38-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1c38-116">Application</span></span>|<span data-ttu-id="f1c38-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1c38-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1c38-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1c38-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="f1c38-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1c38-119">Request headers</span></span>
|<span data-ttu-id="f1c38-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1c38-120">Header</span></span>|<span data-ttu-id="f1c38-121">値</span><span class="sxs-lookup"><span data-stu-id="f1c38-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1c38-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1c38-122">Authorization</span></span>|<span data-ttu-id="f1c38-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f1c38-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1c38-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f1c38-124">Accept</span></span>|<span data-ttu-id="f1c38-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1c38-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1c38-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1c38-126">Request body</span></span>
<span data-ttu-id="f1c38-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f1c38-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f1c38-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="f1c38-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f1c38-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1c38-129">Property</span></span>|<span data-ttu-id="f1c38-130">型</span><span class="sxs-lookup"><span data-stu-id="f1c38-130">Type</span></span>|<span data-ttu-id="f1c38-131">説明</span><span class="sxs-lookup"><span data-stu-id="f1c38-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1c38-132">appleId</span><span class="sxs-lookup"><span data-stu-id="f1c38-132">appleId</span></span>|<span data-ttu-id="f1c38-133">String</span><span class="sxs-lookup"><span data-stu-id="f1c38-133">String</span></span>|<span data-ttu-id="f1c38-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f1c38-134">Not yet documented</span></span>|
|<span data-ttu-id="f1c38-135">deptoken</span><span class="sxs-lookup"><span data-stu-id="f1c38-135">depToken</span></span>|<span data-ttu-id="f1c38-136">String</span><span class="sxs-lookup"><span data-stu-id="f1c38-136">String</span></span>|<span data-ttu-id="f1c38-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f1c38-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f1c38-138">応答</span><span class="sxs-lookup"><span data-stu-id="f1c38-138">Response</span></span>
<span data-ttu-id="f1c38-139">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f1c38-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f1c38-140">例</span><span class="sxs-lookup"><span data-stu-id="f1c38-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1c38-141">要求</span><span class="sxs-lookup"><span data-stu-id="f1c38-141">Request</span></span>
<span data-ttu-id="f1c38-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f1c38-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="f1c38-143">応答</span><span class="sxs-lookup"><span data-stu-id="f1c38-143">Response</span></span>
<span data-ttu-id="f1c38-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f1c38-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





