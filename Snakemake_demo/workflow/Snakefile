dataset = "genus"
method = "glmnet"
seed = 1001

rule trail_ml_model:
    input:
        R="workflow/scripts/train_ml.R",
        csv=f"data/{dataset}.csv"
    output:
        model=f"results/{dataset}/runs/{method}_{seed}_model.Rds"
    script:
        "scripts/train_ml.R"