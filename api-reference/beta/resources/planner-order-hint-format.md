---
title: Planner でオーダー ヒントを使用する
description: '`)'
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 6d88fa821aba48538c102ba439439fe22a4d686f
ms.sourcegitcommit: 6720736406f21e40914b27ba28387adedf97fa56
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/12/2019
ms.locfileid: "35639193"
---
# <a name="using-order-hints-in-planner"></a><span data-ttu-id="83e2f-103">Planner でオーダー ヒントを使用する</span><span class="sxs-lookup"><span data-stu-id="83e2f-103">Using order hints in Planner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83e2f-104">オーダー ヒントによって、Planner 内のオブジェクトの並べ替え順序を特定します。</span><span class="sxs-lookup"><span data-stu-id="83e2f-104">Objects in Planner identify their sort order by order hints.</span></span> <span data-ttu-id="83e2f-105">オーダー ヒントの値は文字列です。</span><span class="sxs-lookup"><span data-stu-id="83e2f-105">The order hint values are strings.</span></span> <span data-ttu-id="83e2f-106">クライアントは項目の順序を特定するため、文字の序数値に基づいて文字列を並べ替えることができます。</span><span class="sxs-lookup"><span data-stu-id="83e2f-106">The clients can sort the strings based on ordinal value of characters in them to identify the order of items.</span></span> <span data-ttu-id="83e2f-107">文字の序数値に違いが発生するまで、または文字列の終わりまで、文字列の先頭から文字を比較します。後者の場合、短い方の文字列を長い文字列より前に並べ替えます。</span><span class="sxs-lookup"><span data-stu-id="83e2f-107">The characters are compared from the beginning of the string, until a difference is encountered in the ordinal values of characters, or one string ends, in which case the shorter string would be sorted before the longer.</span></span> <span data-ttu-id="83e2f-108">値には、32 (スペース) から 126 (`~`) の序数のうち、どの文字でも含めることができます</span><span class="sxs-lookup"><span data-stu-id="83e2f-108">The values can contain any character between ordinals 32 (space) and 126 (`~`)</span></span>

<span data-ttu-id="83e2f-109">一例として、オーダー ヒント `a` (序数値 97) を持つ項目は、オーダー ヒント `z` (序数値 122) を持つ別の項目より前に配置されます。</span><span class="sxs-lookup"><span data-stu-id="83e2f-109">As an example, an item with order hint `a` (ordinal value 97) would be placed before another item with order hint `z` (ordinal value 122).</span></span> <span data-ttu-id="83e2f-110">オーダー ヒント `abc` (序数値 97、98、99) を持つ項目は、オーダー ヒント `abd` (序数値 97、98、100) を持つ別の項目より前に配置されます。</span><span class="sxs-lookup"><span data-stu-id="83e2f-110">An item with order hint `abc` (ordinal values 97, 98, 99), would be placed before another item with order hint `abd` (ordinal values 97, 98, 100).</span></span> <span data-ttu-id="83e2f-111">オーダー ヒント `a` を持つ項目は、オーダー ヒント `ab` を持つ別の項目より前に配置されますが、これはすべての既存の文字が同じであり、`a` の方が短いためです。</span><span class="sxs-lookup"><span data-stu-id="83e2f-111">An item with order hint `a` would be placed before another item with order hint `ab` since all existing characters are the same, and `a` is shorter.</span></span>

<span data-ttu-id="83e2f-112">このサービスにより、すべてのオーダー ヒントの値を計算します。</span><span class="sxs-lookup"><span data-stu-id="83e2f-112">The values for all order hints are calculated by the service.</span></span> <span data-ttu-id="83e2f-113">クライアントは、2 つの項目間を移動した項目のオーダー ヒントを指定することによって、項目を並べ替えることができます。オーダー ヒントを次の値に設定します。`<previous order hint> <next order hint>!`、ここでは新しく要求した場所の前に来る項目のオーダー ヒントによって `<previous order hint>` が置き換えられ、新しく要求した場所の後に来る項目のオーダー ヒントによって `<next order hint>` が置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="83e2f-113">The client can reorder items by specifying the order hint for the item that got moved between two items with by setting the order hint to the following value: `<previous order hint> <next order hint>!`, where `<previous order hint>` is to be replaced by the order hint of the item that comes before the new desired location, and `<next order hint>` is to be replaced by the order hint of the item that comes after the new desired location.</span></span> <span data-ttu-id="83e2f-114">これらのオーダー ヒントの値の間には空白文字があり、値全体の後に `!` が付きます。</span><span class="sxs-lookup"><span data-stu-id="83e2f-114">There is a space character between these order hint values, and the entire value is suffixed with `!`.</span></span> <span data-ttu-id="83e2f-115">いずれの項目も存在しない場合は、代わりに空の文字列を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="83e2f-115">If either item isn't present, empty string should be used instead.</span></span> <span data-ttu-id="83e2f-116">この値は以前の計算で構成することもでき、オーダー ヒントを返したサービスと全く同じように項目を並べ替えるためにクライアントで使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="83e2f-116">This value can also be composed of previous calculations, and can be used in the client to sort items exactly like service returned order hints.</span></span> <span data-ttu-id="83e2f-117">更新プログラムでクライアントがこれらの値を送信したら、このサービスは要求された場所で並べ替えを行う短い値を計算します。</span><span class="sxs-lookup"><span data-stu-id="83e2f-117">Once the client sends these values in an update, the service will calculate a short value that sorts in the desired location.</span></span>

> <span data-ttu-id="83e2f-118">**注:** 次の例では、実際の順序のヒントの値は、わかりやすく`'`するために一重引用符 () で囲まれています。ただし、データの一部ではないため、サービスに送信することはできません。</span><span class="sxs-lookup"><span data-stu-id="83e2f-118">**Note:** In the following examples, the actual order hint values are surrounded in single quote characters (`'`) for clarity, however these are not part of the data, and must not be sent to the service.</span></span>
 
<span data-ttu-id="83e2f-119">たとえば、以下のオーダー ヒントの並べ替えのリストについて検討します。</span><span class="sxs-lookup"><span data-stu-id="83e2f-119">As an example, consider the following list of sorted order hints:</span></span>

1. <span data-ttu-id="83e2f-120">項目 1 (オーダー ヒント: `'5637'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-120">Item 1 (Order Hint: `'5637'`)</span></span>
2. <span data-ttu-id="83e2f-121">項目 2 (オーダー ヒント: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-121">Item 2 (Order Hint: `'adhg'`)</span></span>

<span data-ttu-id="83e2f-122">項目 3 を項目 1 の前に配置し、次に項目 4 を項目 1 と項目 2 の間に配置します。次いで項目 5 を項目 2 の後に配置すれば、クライアント上で以下のオーダー ヒントが作成されます。</span><span class="sxs-lookup"><span data-stu-id="83e2f-122">Placing an Item 3 before Item 1, then placing item 4 between Item 1 and Item 2, and then placing item 5 after Item 2, would create the following order hints on the client.</span></span> 

1. <span data-ttu-id="83e2f-123">項目 3 (オーダー ヒント: `' 5637!'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-123">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="83e2f-124">項目 1 (オーダー ヒント: `'5637'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-124">Item 1 (Order Hint: `'5637'`)</span></span>
3. <span data-ttu-id="83e2f-125">項目 4 (オーダー ヒント: `'5637 adhg!'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-125">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="83e2f-126">項目 2 (オーダー ヒント: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-126">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="83e2f-127">項目 5 (オーダー ヒント: `'adhg !'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-127">Item 5 (Order Hint: `'adhg !'`)</span></span>

<span data-ttu-id="83e2f-128">次に、項目 1 をリストの末尾に移動すると、次のオーダー ヒントが生成されます。</span><span class="sxs-lookup"><span data-stu-id="83e2f-128">Then, moving item 1 to the end of the list would generate:</span></span>

1. <span data-ttu-id="83e2f-129">項目 3 (オーダー ヒント: `' 5637!'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-129">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="83e2f-130">項目 4 (オーダー ヒント: `'5637 adhg!'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-130">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
3. <span data-ttu-id="83e2f-131">項目 2 (オーダー ヒント: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-131">Item 2 (Order Hint: `'adhg'`)</span></span>
4. <span data-ttu-id="83e2f-132">項目 5 (オーダー ヒント: `'adhg !'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-132">Item 5 (Order Hint: `'adhg !'`)</span></span>
5. <span data-ttu-id="83e2f-133">項目 1 (オーダー ヒント: `'adhg ! !'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-133">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="83e2f-134">最後に、項目 5 を項目 3 と項目 4 の間に移動すると、次のオーダー ヒントが生成されます。</span><span class="sxs-lookup"><span data-stu-id="83e2f-134">Finally moving Item 5 between Item 3 and Item 4 would generate:</span></span>

1. <span data-ttu-id="83e2f-135">項目 3 (オーダー ヒント: `' 5637!'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-135">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="83e2f-136">項目 5 (オーダー ヒント: `' 5637! 5637 adhg!!'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-136">Item 5 (Order Hint: `' 5637! 5637 adhg!!'`)</span></span>
3. <span data-ttu-id="83e2f-137">項目 4 (オーダー ヒント: `'5637 adhg!'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-137">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="83e2f-138">項目 2 (オーダー ヒント: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-138">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="83e2f-139">項目 1 (オーダー ヒント: `'adhg ! !'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-139">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="83e2f-140">オーダーヒントの値に対するこれらの変更がパッチ要求でサービスに送信されると、サービスはクライアントが意図した順序を保持する適切な値を計算します。</span><span class="sxs-lookup"><span data-stu-id="83e2f-140">When these changes to order hint values are sent to the service in patch requests, the service will calculate proper values that keep the order intended by the client.</span></span> <span data-ttu-id="83e2f-141">クライアントは、 `Prefer: return=representation` `PATCH`要求で設定ヘッダーが指定されている場合、すぐに値を取得できます。</span><span class="sxs-lookup"><span data-stu-id="83e2f-141">The client can obtain the values immediate if the `Prefer: return=representation` preference header is specified in the `PATCH` requests.</span></span> <span data-ttu-id="83e2f-142">上記の場合の値は、次のように表示されます (実際の値は異なる場合があります)。</span><span class="sxs-lookup"><span data-stu-id="83e2f-142">The values for the case above may look like the following (the actual values may differ).</span></span> 

1. <span data-ttu-id="83e2f-143">項目 3 (オーダー ヒント: `'432b'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-143">Item 3 (Order Hint: `'432b'`)</span></span>
2. <span data-ttu-id="83e2f-144">項目 5 (オーダー ヒント: `'6F"#'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-144">Item 5 (Order Hint: `'6F"#'`)</span></span>
3. <span data-ttu-id="83e2f-145">項目 4 (オーダー ヒント: `'7A$6'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-145">Item 4 (Order Hint: `'7A$6'`)</span></span>
4. <span data-ttu-id="83e2f-146">項目 2 (オーダー ヒント: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-146">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="83e2f-147">項目 1 (オーダー ヒント: `'de5%'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-147">Item 1 (Order Hint: `'de5%'`)</span></span>

<span data-ttu-id="83e2f-148">リストの最初の項目を作成する場合、前または次の項目がいずれも存在しないため、オーダー ヒントを `!` として指定することができます。ただし、項目の作成時にオーダー ヒントの値が指定されない場合、そうする必要はありません。これは、サービスが項目のすべてのオーダー ヒントの値を自動生成するためです。</span><span class="sxs-lookup"><span data-stu-id="83e2f-148">Order Hints can be specified for creating the first item in the list as `!`, since neither a previous or a next item exists in that case, however this is unnecessary, as the service will auto-generate values for all order hint values on items if they are not specified during creation of the item.</span></span> <span data-ttu-id="83e2f-149">次の例は、以前に空白だったリストに項目を配置する場合、オーダー ヒントを使用する必要があることを示しています。</span><span class="sxs-lookup"><span data-stu-id="83e2f-149">Following example illustrates the order hints should be used when placing items in a previously empty list.</span></span>
<span data-ttu-id="83e2f-150">最初の項目を追加します。</span><span class="sxs-lookup"><span data-stu-id="83e2f-150">Add the first item:</span></span>

1. <span data-ttu-id="83e2f-151">項目 1 (オーダー ヒント: `' !'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-151">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="83e2f-152">2 番目の項目を先頭に追加します。</span><span class="sxs-lookup"><span data-stu-id="83e2f-152">Add the second item to top:</span></span>

1. <span data-ttu-id="83e2f-153">項目 2 (オーダー ヒント: `'  !!'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-153">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="83e2f-154">項目 1 (オーダー ヒント: `' !'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-154">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="83e2f-155">3 番目の項目を一番下に追加します。</span><span class="sxs-lookup"><span data-stu-id="83e2f-155">Add the third item to bottom:</span></span>

1. <span data-ttu-id="83e2f-156">項目 2 (オーダー ヒント: `'  !!'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-156">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="83e2f-157">項目 1 (オーダー ヒント: `' !'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-157">Item 1 (Order Hint: `' !'`)</span></span>
3. <span data-ttu-id="83e2f-158">項目 3 (オーダー ヒント: `' ! !'`)</span><span class="sxs-lookup"><span data-stu-id="83e2f-158">Item 3 (Order Hint: `' ! !'`)</span></span>







