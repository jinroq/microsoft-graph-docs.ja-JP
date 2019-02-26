---
title: Delete deviceCategory
description: deviceCategory を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 35dffc1c280caeb10007dbf11d390ac7487d4a61
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30249971"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="01fcc-103">Delete deviceCategory</span><span class="sxs-lookup"><span data-stu-id="01fcc-103">Delete deviceCategory</span></span>

> <span data-ttu-id="01fcc-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="01fcc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01fcc-105">[deviceCategory](../resources/intune-shared-devicecategory.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="01fcc-105">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01fcc-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="01fcc-106">Prerequisites</span></span>
<span data-ttu-id="01fcc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="01fcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01fcc-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="01fcc-109">Permission type</span></span>|<span data-ttu-id="01fcc-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="01fcc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01fcc-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="01fcc-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="01fcc-112">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="01fcc-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="01fcc-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01fcc-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="01fcc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="01fcc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01fcc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="01fcc-115">Not supported.</span></span>|
|<span data-ttu-id="01fcc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="01fcc-116">Application</span></span>|<span data-ttu-id="01fcc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="01fcc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01fcc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="01fcc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="01fcc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="01fcc-119">Request headers</span></span>
|<span data-ttu-id="01fcc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="01fcc-120">Header</span></span>|<span data-ttu-id="01fcc-121">値</span><span class="sxs-lookup"><span data-stu-id="01fcc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01fcc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="01fcc-122">Authorization</span></span>|<span data-ttu-id="01fcc-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="01fcc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01fcc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="01fcc-124">Accept</span></span>|<span data-ttu-id="01fcc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="01fcc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01fcc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="01fcc-126">Request body</span></span>
<span data-ttu-id="01fcc-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="01fcc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01fcc-128">応答</span><span class="sxs-lookup"><span data-stu-id="01fcc-128">Response</span></span>
<span data-ttu-id="01fcc-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="01fcc-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="01fcc-130">例</span><span class="sxs-lookup"><span data-stu-id="01fcc-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="01fcc-131">要求</span><span class="sxs-lookup"><span data-stu-id="01fcc-131">Request</span></span>
<span data-ttu-id="01fcc-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="01fcc-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="01fcc-133">応答</span><span class="sxs-lookup"><span data-stu-id="01fcc-133">Response</span></span>
<span data-ttu-id="01fcc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="01fcc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



