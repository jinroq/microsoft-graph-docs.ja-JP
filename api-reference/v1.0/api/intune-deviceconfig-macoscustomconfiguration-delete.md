---
title: Delete macOSCustomConfiguration
description: macOSCustomConfiguration を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 90ef02d23779397c3dc6cba3af70b7bc86d794e3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262812"
---
# <a name="delete-macoscustomconfiguration"></a><span data-ttu-id="23ce1-103">Delete macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="23ce1-103">Delete macOSCustomConfiguration</span></span>

> <span data-ttu-id="23ce1-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="23ce1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23ce1-105">[macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="23ce1-105">Deletes a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23ce1-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="23ce1-106">Prerequisites</span></span>
<span data-ttu-id="23ce1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23ce1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="23ce1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="23ce1-109">Permission type</span></span>|<span data-ttu-id="23ce1-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="23ce1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23ce1-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="23ce1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="23ce1-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23ce1-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23ce1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="23ce1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23ce1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23ce1-114">Not supported.</span></span>|
|<span data-ttu-id="23ce1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="23ce1-115">Application</span></span>|<span data-ttu-id="23ce1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23ce1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23ce1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="23ce1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="23ce1-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23ce1-118">Request headers</span></span>
|<span data-ttu-id="23ce1-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23ce1-119">Header</span></span>|<span data-ttu-id="23ce1-120">値</span><span class="sxs-lookup"><span data-stu-id="23ce1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23ce1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="23ce1-121">Authorization</span></span>|<span data-ttu-id="23ce1-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="23ce1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23ce1-123">承諾</span><span class="sxs-lookup"><span data-stu-id="23ce1-123">Accept</span></span>|<span data-ttu-id="23ce1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="23ce1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23ce1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="23ce1-125">Request body</span></span>
<span data-ttu-id="23ce1-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="23ce1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23ce1-127">応答</span><span class="sxs-lookup"><span data-stu-id="23ce1-127">Response</span></span>
<span data-ttu-id="23ce1-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="23ce1-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="23ce1-129">例</span><span class="sxs-lookup"><span data-stu-id="23ce1-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="23ce1-130">要求</span><span class="sxs-lookup"><span data-stu-id="23ce1-130">Request</span></span>
<span data-ttu-id="23ce1-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="23ce1-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="23ce1-132">応答</span><span class="sxs-lookup"><span data-stu-id="23ce1-132">Response</span></span>
<span data-ttu-id="23ce1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="23ce1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



