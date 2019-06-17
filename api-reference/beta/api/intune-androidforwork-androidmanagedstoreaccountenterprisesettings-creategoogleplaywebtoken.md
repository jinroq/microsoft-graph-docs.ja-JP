---
title: createGooglePlayWebToken アクション
description: 埋め込みコンポーネントで使用される web トークンを生成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 31318c40894f861832a99c7de43f64b6a7e3c64e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34965509"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="40e57-103">createGooglePlayWebToken アクション</span><span class="sxs-lookup"><span data-stu-id="40e57-103">createGooglePlayWebToken action</span></span>

> <span data-ttu-id="40e57-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40e57-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40e57-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="40e57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40e57-106">埋め込みコンポーネントで使用される web トークンを生成します。</span><span class="sxs-lookup"><span data-stu-id="40e57-106">Generates a web token that is used in an embeddable component.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40e57-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="40e57-107">Prerequisites</span></span>
<span data-ttu-id="40e57-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40e57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40e57-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40e57-110">Permission type</span></span>|<span data-ttu-id="40e57-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="40e57-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40e57-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40e57-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40e57-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40e57-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="40e57-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40e57-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40e57-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40e57-115">Not supported.</span></span>|
|<span data-ttu-id="40e57-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40e57-116">Application</span></span>|<span data-ttu-id="40e57-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40e57-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40e57-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40e57-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="40e57-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40e57-119">Request headers</span></span>
|<span data-ttu-id="40e57-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40e57-120">Header</span></span>|<span data-ttu-id="40e57-121">値</span><span class="sxs-lookup"><span data-stu-id="40e57-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40e57-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="40e57-122">Authorization</span></span>|<span data-ttu-id="40e57-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="40e57-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40e57-124">承諾</span><span class="sxs-lookup"><span data-stu-id="40e57-124">Accept</span></span>|<span data-ttu-id="40e57-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40e57-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40e57-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="40e57-126">Request body</span></span>
<span data-ttu-id="40e57-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="40e57-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="40e57-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="40e57-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="40e57-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40e57-129">Property</span></span>|<span data-ttu-id="40e57-130">型</span><span class="sxs-lookup"><span data-stu-id="40e57-130">Type</span></span>|<span data-ttu-id="40e57-131">説明</span><span class="sxs-lookup"><span data-stu-id="40e57-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40e57-132">parentUri</span><span class="sxs-lookup"><span data-stu-id="40e57-132">parentUri</span></span>|<span data-ttu-id="40e57-133">String</span><span class="sxs-lookup"><span data-stu-id="40e57-133">String</span></span>|<span data-ttu-id="40e57-134">コンポーネントをホストしているページの https パス。</span><span class="sxs-lookup"><span data-stu-id="40e57-134">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="40e57-135">応答</span><span class="sxs-lookup"><span data-stu-id="40e57-135">Response</span></span>
<span data-ttu-id="40e57-136">成功した場合、この関数は `200 OK` 応答コードと、応答本文で String を返します。</span><span class="sxs-lookup"><span data-stu-id="40e57-136">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40e57-137">例</span><span class="sxs-lookup"><span data-stu-id="40e57-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="40e57-138">要求</span><span class="sxs-lookup"><span data-stu-id="40e57-138">Request</span></span>
<span data-ttu-id="40e57-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="40e57-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="40e57-140">応答</span><span class="sxs-lookup"><span data-stu-id="40e57-140">Response</span></span>
<span data-ttu-id="40e57-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="40e57-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```





